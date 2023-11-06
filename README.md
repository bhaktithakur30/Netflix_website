# Netflix_website
I developed this latest netflix website using HTML ,  and CSS . To see the website visit https://imbhaktithakur.me/
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>Netflix Clone</title>
    <style>
        /* Reset some default styles */
*{
    margin: 0;
    padding: 0;
    font-family: 'poppins',sans-serif;
    box-sizing: border-box;
}
body{
    background: #000;
    color: #fff;
}
.header{
    width: 100%;
    height: 100vh;
    background-image: linear-gradient(rgba(0,0,0,0.7),rgba(0,0,0,0.7)),url("https://th.bing.com/th/id/R.d2edb29f3f970c36aadecbb01ed0bb79?rik=z%2bAuuobpN0KNSg&riu=http%3a%2f%2fisquad.tv%2fwp-content%2fuploads%2f2018%2f08%2fNetflix-Background.jpg&ehk=Ij4PSd%2bZkTcESSlAVWoGpNmExM0fu3BgteNT6AnS9lM%3d&risl=&pid=ImgRaw&r=0");
    background-size: cover;
    background-position: center;
    padding: 10px 8%;
    position: relative;
}


nav {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 10px 0;
}
.logo{
    width: 14%;
    cursor: pointer;
}
nav button{
    border: 0;
    outline: 0;
    background: #db0001;
    color: #fff;
    padding: 7px 20px;
    font-size: 12px;
    border-radius: 4px;
    margin-left: 10px;
    cursor: pointer;
}

.language-btn{
    border: 1px solid #fff;
    background: transparent;
}

.header-content{
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%,-50%);
    text-align: center;
    margin-top: 100px;
}

.header-content h1{
    font-size: 60px;
    line-height: 70px;
    font-weight: 600;
    max-width: 650px;
}
.header-content h3{
    font-weight: 400;
    margin-bottom: 20px;
}

.email-signup{
    background: #fff;
    border-radius: 4px;
    display: flex;
    align-items: center;
    margin-top: 30px;
    overflow: hidden;
}

.email-signup input{
    flex: 1;
    border: 0;
    outline: 0;
    margin-left: 20px;
}
.email-signup button{
    background: #db0001;
    border: 0;
    outline: 0;
    color: #fff;
    font-size: 16px;
    cursor: pointer;
    padding: 15px 30px;
}

/*---------features--------*/

.features{
    padding: 50px 12%;
    font-size: 22px;
}
.row{
    display: flex;
    width: 100%;
    align-items: center;
    flex-wrap: wrap;
    padding: 50px 0;
}
    
.text-col{
    flex-basis: 50%;
    margin-bottom: 20px;
}
.img-col{
    flex-basis: 50%;
    margin-bottom: 20px;
}
.img-col img{
    display: block;
    width: 90%;
    margin: auto;
}

.features h2{
    font-size: 50px;
    font-weight: 600;
    margin-bottom: 20px;
}

/*----------faq---------*/
.faq{
    padding: 10px 12%;
    text-align: center;
    font-size: 18px;
}

.faq h3{
    font-weight: 500;
    font-size: 35px;
}

.accordion{
    margin: 60px auto ;
    width: 100%;
    max-width: 750px;
}
.accordion li{
    list-style: none;
    width: 100%;
    padding: 5px;
}
.accordion li label{
    display: flex;
    align-items: center;
    padding: 20px;
    font-size: 18px;
    font-weight: 500;
    background: #303030;
    margin-bottom:  2px;
    cursor: pointer;
    position: relative;
}
label::after{
    content: '+';
    font-size: 34px;
    position: absolute;
    right: 20px;
    transition: transform 0.5s;
}
input[type="radio"]{
    display: none;
}
.accordion .content{
    background: #303030;
    text-align: left;
    padding: 0 20px;
    max-height: 0;
    overflow: hidden;
    transition: max-height 0.5s, padding 0.5s;
}
.accordion input[type="radio"]:checked + label + .content{
    max-height: 600px;
    padding: 30px 20px;
}
.faq .email-signup{
    max-width: 600px;
    margin: 20px autp 60px;
}
.faq small{
    font-size: 13px;
}

/*---------footer-------*/
.footer{
    padding: 50px 15% 10px;
    border-top: 6px solid #333;
    color: #777;
}
.footer h2{
    font-size: 18px;
    font-weight: 400;
    margin-bottom: 30px;
}
.footer .col{
    flex-basis: 25%;
    flex-grow: 1;
    margin-bottom: 20px;
}
.footer .col a{
    display: block;
    text-decoration: none;
    color: #777;
    font-size: 14px;
    margin-bottom: 10px;
}
.footer .row{
    align-items: flex-start;
    padding: 10px 0;
}
.footer .language-btn{
    color: #fff;
    padding: 10px 20px;
    border-radius: 3px;
}
.copyright-txt{
    font-size: 14px;
    margin-top: 20px;
    margin-bottom:10px;
}
 /*------media-queries-for-small-screen------*/
 @media only screen and (max-width: 600px){
    .logo{
        width: 100px;
    }
    nav button{
        padding: 5px 10px;
    }
    nav .language-btn{
        padding: 4px 8px;
    }
    .header-content{
        position: unset;
        transform: none;
        padding-top: 150px;
    }
    .header-content h1{
        font-size: 30px;
    }
    .email-signup button{
        font-size: 12px;
        padding: 10px 15px;
    }
    .text-col, .img-col{
        flex-basis: 100%;
    }
    .features h2{
        font-size: 30px;
    }
    .features p{
        font-size: 15px;
    }
    .row:nth-child(2), .row:nth-child(4){
        flex-direction: column-reverse;
    }
    .features .row{
        padding: 10px 0;
    }
    .faq h2{
        font-size: 20px;
    }
    .accordion .content{
        font-size: 14px;
    }
    .accordion li label{
        padding: 10px;
        font-size: 14px;
    }
    label::after{
        font-size: 22px;
    }
 }
    </style>
</head>
<body> 
  <div class="header">
    <nav>
        <img class="logo" src="https://logodownload.org/wp-content/uploads/2014/10/netflix-logo.png "/>
         <div>
            <button class="language-btn">English</button>
            <button>Sign In</button>
        </div>
    </nav>
    <div class="header-content">
        <h1>Unlimited movies, TV shows and more.</h1>
        <h3>Watch anywhere. Cancle anytime.</h3>
        <p>Ready to watch? Enter your email to create or restart your membership.</p>
        <form class="email-signup">
            <input type="email" placeholder="Email address" required>
            <button type="submit">Get Started</button>
        </form>
    </div>
  </div>

  <div class="features">
    <div class="row">
        <div class="text-col">
            <h2>Enjoy on your TV.</h2>
            <p>Watch on smart TVs, Playstation, Xbox, Chromecast, Apple TV, Blu-ray
            players and more.</p>
        </div>
        <div class="img-col">
            <img src="https://i.ytimg.com/vi/atEnIgFbrbQ/maxresdefault.jpg">
        </div>
    </div>
  
   <div class="row">
        <div class="img-col">
            <img src="https://neflix-clone-project.vercel.app/images/strangerthings.png">
        </div>
         <div class="text-col">
            <h2>Downlode your shows to watch offline.</h2>
            <p>Save your favourites easily and always have something to watch.</p>
         </div>
        </div>

       <div class="row">
        <div class="text-col">
             <h2>Watch everywhere.</h2>
             <p>Stream unlimited movies and  TV shows on your phone, tablet, laptop, and 
                TV.</p>
         </div>
            <div class="img-col">
                <img src="https://lh5.googleusercontent.com/proxy/jta6I4Ql7XVERWyKlzpa5g_CkQjS_kMxp7GHuFEBjXRTRg5nJbs45CaAvTgmtbknhDtc0jTfuAJ7l-DfpKhgYS_Cde4NFC-bjZo6YJDI8wJ1uSfFo7C_btrqkQ=w1200-h630-p-k-no-nu">
            </div>
        </div>

     <div class="row">
            <div class="img-col">
                <img src="https://subham2942.github.io/Netflix-sign-In-Clone/images/children.png">
             </div>
            <div class="text-col">
             <h2>Create profiles for children.</h2>
             <p>Send children on adventures with their favourites characters in a space
                made just for them-free with your membership.</p>
         </div>
        </div>
   
  <div class="faq">
    <h2>Frequently Asked Questions</h2>
    <ul class="accordion">
        <li>
            
            
            <label for="first">What is Netflix?</label>
            <div class="content">
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.
                 Asperiores sit deserunt, quae, unde esse quaerat nulla vel
                 molestiae cum explicabo repellendus officiis quos, ipsam maiores provident.
                 Sunt vitae quo exercitationem.</p>
            </div>
        </li>

        <li>
            
            
            <label for="second">How much does Netflix cost?</label>
            <div class="content">
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.
                 Asperiores sit deserunt, quae, unde esse quaerat nulla vel
                 molestiae cum explicabo repellendus officiis quos, ipsam maiores provident.
                 Sunt vitae quo exercitationem.</p>
            </div>
        </li> 
        
        <li>
            
            
            <label for="third">Where can I watch?</label>
            <div class="content">
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.
                 Asperiores sit deserunt, quae, unde esse quaerat nulla vel
                 molestiae cum explicabo repellendus officiis quos, ipsam maiores provident.
                 Sunt vitae quo exercitationem.</p>
            </div>
        </li> 

        <li>
            
            
            <label for="fouth">How do I cancle?</label>
            <div class="content">
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.
                 Asperiores sit deserunt, quae, unde esse quaerat nulla vel
                 molestiae cum explicabo repellendus officiis quos, ipsam maiores provident.
                 Sunt vitae quo exercitationem.</p>
            </div>
        </li> 

        <li>
            
            
            <label for="fifth">What can I watch on Netflix?</label>
            <div class="content">
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.
                 Asperiores sit deserunt, quae, unde esse quaerat nulla vel
                 molestiae cum explicabo repellendus officiis quos, ipsam maiores provident.
                 Sunt vitae quo exercitationem.</p>
            </div>
        </li>

        <li>
            
            
            <label for="sixth">Is Netflix good for kids?</label>
            <div class="content">
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.
                 Asperiores sit deserunt, quae, unde esse quaerat nulla vel
                 molestiae cum explicabo repellendus officiis quos, ipsam maiores provident.
                 Sunt vitae quo exercitationem.</p>
            </div>
        </li>
   </ul>
   <small>Ready to watch? Enter your email to create or restart your membership.</small>
<form class="email-signup">
    <input type="email" placeholder="Email address" required>
    <button type="submit">Get Started</button>
  </form>
 </div>
  
<div class="footer">
    <h3>Questions? call 000-000-000-000</h3>

    <div class="row">
        <div class="col">
            <a href="#">FAQ</a>
            <a href="#">Investor Relations</a>
            <a href="#">Privacy</a>
            <a href="#">Speed Test</a>
        </div>

        <div class="col">
            <a href="#">Help Center</a>
            <a href="#">Jobs</a>
            <a href="#">Cookies Preferences</a>
            <a href="#">Legal Notices</a>
        </div>

        <div class="col">
            <a href="#">Account</a>
            <a href="#">Ways to watch</a>
            <a href="#">Corporate Information</a>
            <a href="#">Only on Netflix</a>
        </div>

        <div class="col">
            <a href="#">Media Center</a>
            <a href="#">Terms of Use</a>
            <a href="#">Contact Us</a>
            
         </div>
    </div>
    <button class="language-btn">English </button>
    <p class="copyright-txt">Netflix India</p>
</div> 
</body>
</html>
