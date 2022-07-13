<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta content="width=device-width, initial-scale=1, maximum-scale=1" name="viewport" />
    <link href="./img/Blue Orange Simple Knight Gaming Logo.png" rel="shortcut icon" />
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
    <title>VIKAS GUPTA</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }

        body {
            background-color: #d3e6f2;
        }

        nav {
            position: sticky;
        }

        #nav {
            overflow: hidden;
            background-color: #c6e8fc;
            width: 100%;
            height: auto;
            display: flex;
            justify-content: space-between;
            box-shadow: #717171;
        }

        #nav a {

            display: block;
            text-align: center;
            padding: 0px 16px;
            text-decoration: none;
            font-size: 17px;
        }

        #nav a:hover {
            /* background-color: #ddd; */
            color: black;
        }

        #nav a.ac {

            color: white;
        }

        .content {
            padding: 16px;
        }

        .sticky {
            position: fixed;
            top: 0;
            width: 100%;
        }

        .sticky+ {
            padding-top: 60px;
        }

        #nav .logo {
            display: inline;
            float: left;
            margin-left: 20px;
            margin-top: 1px;
            width: 5%;
            border: 2px solid cyan;
            outline: 5px solid blueSS;
            border-radius: 100%;


        }

        #nav .logo img {
            border-radius: 100%;
            width: 100%;
            height: 100%;
            object-fit: fill;

        }

        .option,
        .ac {
            width: 75%;
            float: left;
            margin-top: 10px;
        }

        .option ul {
            text-transform: uppercase;
            list-style: none;
            display: flex;
            justify-content: space-around;
            width: 50%;
            cursor: pointer;
            float: right;
            margin-right: -100px;
            margin-top: 10px;
            color: black;
            font-weight: 800;

        }

        .option ul a {
            color: black;
            font-weight: 800;
        }

        .sidenav {
            visibility: hidden;
        }

        .openbtn {
            float: right;
           visibility: hidden;

        }


        .box {
            width: 100%;
            height: 100%;
            padding: 0 300px;

        }

        .container {
            width: 100%;
            height: 600px;
            background-size: cover;
            background-repeat: no-repeat;
            margin: auto;
            background-image: url(./img/Blue\ Modern\ Corporate\ Computer\ and\ Technology\ Linkedin\ Banner.png);
            border-radius: 0 0 30px 30px;
        }

        .slideshow {
            height: 60%;
            width: 50%;
            border-radius: 100%;
            text-align: center;
            padding-top: 20px;
            margin-left: 200px;


        }

        .slideshow .active {
            background-color: #717171;
        }

        .slide {
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
            background-blend-mode: darken;
        }

        .slide1 {
            background-image: url(./img/vikas1.jpg);
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
            width: 100%;
            height: 100%;
            object-fit: cover;
            border-radius: 100%;
            border-left: 5px solid rgb(107, 24, 162);
            border-right: 5px solid rgb(195, 242, 7);

        }

        .slide2 {
            background-image: url(./img/Blue\ Orange\ Simple\ Knight\ Gaming\ Logo.png);
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
            width: 100%;
            height: 100%;
            object-fit: cover;
            border-radius: 100%;
            border-left: 5px solid red;
            border-right: 5px solid yellow;

        }

        .slide2 .active {
            background-color: #717171;
        }

        .fade {
            animation-name: fade;
            animation-duration: 3s;
        }

        .content {
            margin: 0 90px;
            width: 100%;
        }

        .content i {
            font-size: 60px;
            color: lightblue;
            text-shadow: 2px 2px 4px #000000;
            margin-left: 50px;



        }

        #insta {
            margin-left: 30px;
            width: 11%;
            height: auto;
            border-radius: 20px;
            text-align: center;
            text-shadow: 2px 2px 4px #000000;
        }

        #insta:hover {
            color: #fff;
            background: radial-gradient(circle at 30% 107%, #fdf497 0%, #fdf497 5%, #fd5949 45%, #d6249f 60%, #285AEB 90%);
            box-shadow: 0px 3px 10px rgba(0, 0, 0, .25);
        }

        #fb {
            margin-left: 30px;
            width: 13%;
            height: 10%;
            border-radius: 40px;
            text-align: center;
            text-shadow: 2px 2px 4px #000000;
        }

        #fb:hover {
            color: #fff;
            background: linear-gradient(#17A9FD 20%, #0165E1 50%);
            box-shadow: 0px 3px 10px rgba(0, 0, 0, .25);
        }

        #in {
            margin-left: 30px;
            width: 14%;
            height: 13%;
            border-radius: 20px;
            text-align: center;
            text-shadow: 2px 2px 4px #000000;
        }

        #in:hover {
            color: #fff;
            background: #0e76a8;
            box-shadow: 0px 3px 10px rgba(0, 0, 0, .25);
        }

        #tw {
            margin-left: 30px;
            width: 14%;
            height: 13%;
            border-radius: 20px;
            text-align: center;
            text-shadow: 2px 2px 4px #000000;
        }

        #tw:hover {
            color: #fff;
            background: #00acee;
            box-shadow: 0px 3px 10px rgba(0, 0, 0, .25);
        }


        @media screen and (max-width:1040px) {

            html,
            body {
                margin: 0;
                padding: 0;
                overflow-x: hidden;
                overflow-y: hidden;



            }
        }

        @media screen and (max-width: 1040px) {

            #nav {
                display: block;
                text-align: center;
                transition: all 0.5s ease-out;
                height: 80px;

            }

            #nav .logo {
                width: 5%;
                border: 0px solid cyan;

            }





            .v-class {
                visibility: hidden;
            }


            .box {
                height: auto;
                width: 100%;
                padding: 0 50px;


            }

            .sidenav {
                visibility: visible;
                height: 300px;
                width: 250px;
                position: fixed;

                top: 0;
                right: 0;
                background-color: #111;
                overflow-x: hidden;
                transition: 0.5s;
                padding-top: 60px;
                line-height: 3;
            }

            .sidenav a {
                padding: 8px 8px 8px 32px;
                text-decoration: none;
                font-size: 25px;
                color: #818181;
                display: block;
                transition: 0.3s;
            }

            .sidenav a:hover {
                color: #f1f1f1;
            }

            #nav .sidenav .closebtn {
                position: absolute;
                top: -20px;
                right: 25px;
                font-size: 40px;
                margin-left: 50px;
            }

            .openbtn {
                margin-right: 20px;
                visibility: visible;
            }
        }

        @media screen and (max-width: 580px) {
            #nav .logo img {
                width: 50px;
                height: 100%;
                object-fit: cover;
                float: left;
                margin-top: 20px;

            }

            #nav .sidenav {
                padding-top: 40px;
            }

            #nav .sidenav a {
                font-size: 18px;
            }

           

            .container {
                width: 100%;
                height: 600px;
                background-size: cover;
                background-repeat: no-repeat;
                margin: 0px;
                border-radius: 0 0 30px 30px;
            }
        }

        @media screen and (max-width: 770px) {
            .box {
                padding: 0px;
            }

            .slideshow {
                height: 60%;
                width: 50%;
                border-radius: 100%;
                text-align: center;
                padding-top: 20px;
                margin-top: 80px;
                margin: auto;
            }
        }
    </style>


</head>

<body>
    <nav>
        <div id="nav" class=" h-nav">
            <div class="logo hv">
                <img src="./img/Blue Orange Simple Knight Gaming Logo.png" alt="Erorr to load logo" width="100%"
                    height="auto" />
            </div>
            <div class="option ac v-class h-nav">
                <ul>
                    <li>Hey There Contact-me</li>
                    <li><a href="tel:8448414883">8448414883</a></li>
                    <li><a href="mailto:webdesigner844@gmail.com">Web-Designer
                        </a></li>
                </ul>
            </div>
            <div id="mySidenav" class="sidenav">

                <a href="javascript:void(0)" class="closebtn" onclick="closeNav()">&times;</a>
                <a href="#">Hey There Contact-me</a>
                <a href="tel:8448414883">8448414883</a>
                <a href="mailto:webdesigner844@gmail.com">Web-Designer
                </a>
            </div>
            <span class='openbtn' style="font-size:40px;cursor:pointer" onclick="openNav()">&#9776;</span>
        </div>

    </nav>
    <main>
        <div class="box">
            <div class="container">
                <div class="slideshow">

                    <div class="slide fade slide1 ">
                    </div>

                    <div class="slide fade slide2 ">
                    </div>
                    <div style="text-align:center">
                        <span class="dot"></span>
                        <span class="dot"></span>

                    </div>
                </div>
                <div class="content">
                    <a href="https://www.instagram.com/its_web_designer_2001/"> <i class="fa fa-instagram"
                            id="insta"></i></a>
                    <a href="https://www.facebook.com/profile.php?id=100015785507871"><i class="fa fa-facebook"
                            id="fb"></i></a>
                    <a href="https://www.linkedin.com/in/vikas-gupta-baa28b1b3"><i class="fa fa-linkedin"
                            id="in"></i></a>
                    <a href="https://twitter.com/@vikasgupta844"><i class="fa fa-twitter" id="tw"></i></a>


                </div>



            </div>
        </div>






    </main>
    <script>
        let slideIndex = 0;
        startslide();

        function startslide() {
            let i;
            let silderImages = document.getElementsByClassName("slide");
            let dots = document.getElementsByClassName("dot");
            for (i = 0; i < silderImages.length; i++) {
                silderImages[i].style.display = "none";
            }
            slideIndex++;
            if (slideIndex > silderImages.length) { slideIndex = 1 }
            for (i = 0; i < dots.length; i++) {
                dots[i].className = dots[i].className.replace(" active","");
            }
            silderImages[slideIndex - 1].style.display = "block";
            dots[slideIndex - 1].className += " active";
            setTimeout(startslide, 8100);
        }

        //navbar
        window.onscroll = function () { myFunction() };

        var nav = document.getElementById("nav");
        var sticky = nav.offsetTop;

        function myFunction() {
            if (window.pageYOffset >= sticky) {
                nav.classList.add("sticky")
            } else {
                nav.classList.remove("sticky");
            }
        }

        //burger nav

        function closeNav() {
            document.getElementById("mySidenav").style.width = "0";
        }


        function openNav() {
            document.getElementById("mySidenav").style.width = "250px";
          
        }


    </script>
</body>

</html>
