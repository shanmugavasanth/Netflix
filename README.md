# Netflix
# URL
https://shanmugavasanth.github.io/Netflix/

# Code
```
<!DOCTYPE html>
<html>
<head>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title> Netflix </title>
    <style>
        *{
            margin: 0;
            padding: 0;
            font-family: 'Poppins', sans-serif;
            box-sizing: border-box;
        }

        body{
            background: black;
            color: white;
        }

        .header{
            width: 100%;
            height: 100vh;
            background-image: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), url(images/background.jpg);
            background-size: cover;
            background-position: center;
            padding: 10px 8%;
            position: relative;
            border-bottom: 6px solid #333;
        }

        nav{
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 10px 0;
        }

        .logo{
            width: 150px;
            cursor: pointer;
        }

        nav button{
            border: 0;
            outline: 0;
            background: #db0001;
            color: #fff;
            padding: 7px 20px;
            font-size: 12px;
            border-radius: 5px;
            margin-left: 10px;
            cursor: pointer;
        }

        .l-btn{
            display: inline-flex;
            align-items: center;
            background: transparent;
            border: 1px solid white;
            padding: 7px 10px;
        }

        .l-btn img{
            width: 10px;
            margin-left: 10px;
        }

        .header-content{
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
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

        .email-box{
            background: #fff;
            border-radius: 4px;
            display: flex;
            align-items: center;
            margin-top: 30px;
            overflow: hidden;
        }

        .email-box input{
            flex: 1;
            border: 0;
            outline: 0;
            margin-left: 20px;
        }

        .email-box button{
            background: #db0001;
            border: 0;
            outline: 0;
            color: #fff;
            font-size: 16px;
            cursor: pointer;
            padding: 15px 30px;
        }

        .feature{
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

        .text{
            flex-basis: 50%;
            margin-bottom: 20px;
        }

        .image{
            flex-basis: 50%;
            margin-bottom: 20px
        }

        .image img{
            display: block;
            width: 90%;
            margin: auto;
        }

        .feature h2{
            font-size: 50px;
            font-weight: 600;
            margin-bottom: 20px
        }

        .faq{
            padding: 10px 12%;
            text-align: center;
            font-size: 18px;
            border-top: 6px solid #333;
        }

        .faq h2{
            margin-top: 30px;
            font-weight: 500;
            font-size: 40px;
        }

        .accordion{
            margin: 60px auto;
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
            margin-bottom: 2px;
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

        .accordion input[type="radio"]:checked + label::after{
            transform: rotate(135deg);
        }

        .faq .email-box{
            max-width: 600px;
            margin: 20px auto 60px;
        }

        .faq small{
            font-size: 13px;
        }

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
            margin-bottom: 14px;
        }

        .footer .row{
            align-items: flex-start;
            padding: 10px 0;
        }

        .footer .l-btn{
            color: #fff;
            padding: 10px 20px;
            border-radius: 3px;
        }

        .copyright{
            font-size: 14px;
            margin-top: 20px;
            margin-bottom: 10px;
        }
    </style>
</head>
<body>
<div class="header">
    <nav>
        <img src="images/logo.png" class="logo">
        <div>
            <button class="l-btn"> English <img src="images/down-icon.png"> </button>
            <button> Sign in </button>
        </div>
    </nav>
    <div class="header-content">
        <h1> Unlimited movies, TV shows and more. </h1>
        <h3> Watch anywhere. Cancel anytime. </h3>
        <p> Ready to watch? Enter your email. </p>
        <form class="email-box">
            <input type="email" placeholder="Email address" required>
            <button type="submit"> Get Started </button>
        </form>
    </div>
</div>
<div class="feature">
    <div class="row">
        <div class="text">
            <h2> Enjoy on your TV. </h2>
            <p> Watch on smart TVs, Playstation, Xbox, Chromecast, Apple TV, Blu-ray players and more. </p>
        </div>
        <div class="image">
            <img src="images/feature-1.png" alt="">
        </div>
    </div>
    <div class="row">
        <div class="image">
            <img src="images/feature-2.png" alt="">
        </div>
        <div class="text">
            <h2> Download your shows to watch offline. </h2>
            <p> Save your favourites easily and always have something to watch. </p>
        </div>
    </div>
    <div class="row">
        <div class="text">
            <h2> Watch everywhere. </h2>
            <p> Stream unlimited movies and TV shows on your phone, tablet, laptop and TV. </p>
        </div>
        <div class="image">
            <img src="images/feature-3.png" alt="">
        </div>
    </div>
    <div class="row">
        <div class="image">
            <img src="images/feature-4.png" alt="">
        </div>
        <div class="text">
            <h2> Create profiles for children. </h2>
            <p> Send children on adventures with their favourite characters in a space made just for them--free with your membership. </p>
        </div>
    </div>
</div>
<div class="faq">
    <h2> Frequently Asked Question </h2>
    <ul class="accordion">
        <li>
            <input type="radio" name="accordion" id="first">
            <label for="first"> What is Netflix? </label>
            <div class="content">
                <p> Netflix is a popular streaming service that lets you watch movies, TV shows, documentaries, and more, all online. You can watch it on various devices like smart TVs, computers, smartphones, and tablets. Netflix offers a wide variety of content, including original shows and films, and you can watch them anytime with a subscription. </p>
            </div>
        </li>
        <li>
            <input type="radio" name="accordion" id="second">
            <label for="second"> How much does Netflix cost? </label>
            <div class="content">
                <p> Netflix is a popular streaming service that lets you watch movies, TV shows, documentaries, and more, all online. You can watch it on various devices like smart TVs, computers, smartphones, and tablets. Netflix offers a wide variety of content, including original shows and films, and you can watch them anytime with a subscription. </p>
            </div>
        </li>
        <li>
            <input type="radio" name="accordion" id="third">
            <label for="third"> Where can I watch? </label>
            <div class="content">
                <p> Netflix is a popular streaming service that lets you watch movies, TV shows, documentaries, and more, all online. You can watch it on various devices like smart TVs, computers, smartphones, and tablets. Netflix offers a wide variety of content, including original shows and films, and you can watch them anytime with a subscription. </p>
            </div>
        </li>
        <li>
            <input type="radio" name="accordion" id="fourth">
            <label for="fourth"> How do I cancel? </label>
            <div class="content">
                <p> Netflix is a popular streaming service that lets you watch movies, TV shows, documentaries, and more, all online. You can watch it on various devices like smart TVs, computers, smartphones, and tablets. Netflix offers a wide variety of content, including original shows and films, and you can watch them anytime with a subscription. </p>
            </div>
        </li>
    </ul>
    <small> Ready to watch? Enter your email. </small>
    <form class="email-box">
        <input type="email" placeholder="Email address" required>
        <button type="submit"> Get Started </button>
    </form>
</div>
<div class="footer">
    <h2> Questions? call 8489518892 </h2>
    <div class="row">
        <div class="col">
            <a href="#"> FAQ </a>
            <a href="#"> Investor Relations </a>
            <a href="#"> Privacy </a>
            <a href="#"> Speed Test </a>
        </div>
        <div class="col">
            <a href="#"> Help Center </a>
            <a href="#"> Jobs </a>
            <a href="#"> Cookies </a>
            <a href="#"> Legal Notices </a>
        </div>
        <div class="col">
            <a href="#"> Account </a>
            <a href="#"> Ways to watch </a>
            <a href="#"> Corporate Information </a>
            <a href="#"> Only on Netflix </a>
        </div>
        <div class="col">
            <a href="#"> Media Centre </a>
            <a href="#"> Terms & Condition</a>
            <a href="#"> Contact Us </a>
        </div>
    </div>
    <button class="l-btn"> English <img src="images/down-icon.png"> </button>
    <p class="copyright"> Netflix India </p>
</div>
</body>
</html>
```

# Result

![Screenshot 2024-11-15 193105](https://github.com/user-attachments/assets/b760e5e9-4741-4b59-a387-99c052c19b34)

![Screenshot 2024-11-15 193124](https://github.com/user-attachments/assets/9a7fd095-88d7-4921-9385-29901dad2400)

![Screenshot 2024-11-15 193143](https://github.com/user-attachments/assets/fe4985ea-7dd9-406e-885c-1443bdd793bb)

![Screenshot 2024-11-15 193158](https://github.com/user-attachments/assets/5502a85b-1b7e-48f7-8e65-1775c7a39aca)

![Screenshot 2024-11-15 193215](https://github.com/user-attachments/assets/1b24e07d-44ac-4304-85c1-25346c028a5f)

![Screenshot 2024-11-15 193228](https://github.com/user-attachments/assets/358c5477-7d29-478f-ae27-a5a13439f94b)

![Screenshot 2024-11-15 193242](https://github.com/user-attachments/assets/9a270195-df11-4210-a73e-c9c5b4750d0f)
