@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500;700&display=swap');
:root{
    --btn-color:#e58f00;
    --about-sec:#1d1d23;
}
*{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
    outline: none;
    text-decoration: none;
    font-family: 'Roboto', sans-serif;
    transition: 0.5s;
    text-transform: capitalize;
}
html{
    font-size: 65%;
    scroll-behavior: smooth;
}
.header{
    padding: 1rem 7%;
    position: fixed;
    left: 0;
    right: 0;
    display: flex;
    justify-content: space-between;
    align-items: center;
    z-index: 100;
    background: #1d1d23;
}
.logo img{
    width: 60px;
}
.navbar a{
    color: white;
    margin: 0.5rem;
    padding: 0.5rem;
    font-size: 1.5rem;
}
.navbar a:hover{
    color: var(--btn-color);
}
.icons div{
    color: white;
    font-size: 1.5rem;
    margin-right: 10px;
    display: none;
}
.icons div:hover{
    cursor: pointer;
}

.icons a{
    color: white;
    padding: 0.6rem 1.5rem;
    border: 1px solid rgb(28, 28, 28);
    border-radius: 10px;
    font-size: 18px;
   transition: 0.5s;
   display: inline-block;
}
.contact-btn:hover{
    transform: scale(1.1);
    background: var(--btn-color);
    border: 1px solid white;
}

.navbar.active{
    clip-path: polygon(0 0, 100% 0, 100% 100%, 0% 100%);
}

/* design for home section */

.home{
    padding: 1rem 7%;
    background: url(images/background.png);
    min-height: 100vh;
    height: 100%;
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
}
.main-home{
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    gap: 15px;
    padding-top: 150px;
    padding-left: 4rem;
    padding-right: 4rem;
}
.home-inner-content{
    flex: 1 1 45rem;
}
.home-image{
    width: 100%;
    height: 100%;
    position: relative;
    
}
.home-image img{
    width: 100%;
    position: absolute;
    transform: translate(0%, -28%);
    animation: mymove 5s infinite ease-in-out;
}
@keyframes mymove {
    0%   {top: 0px;}
    50%   {top: 15px;}
    75%   {top: 10px;}
    100%   {top: 0px;}
  }
.home-text-content{
    padding: 0 8rem;
}
.home-text-content h1{
    font-size: 45px;
    color: #e58f00;
}
.home-text-content p{
    color: white;
    font-size: 1.5rem;
    margin-top: 10px;
    margin-bottom: 15px;
    line-height: 25px;
}
.home-text-content a{
    color: white;
    padding: 0.6rem 1.5rem;
    border: 1px solid orange;
    border-radius: 10px;
    font-size: 18px;
   transition: 0.5s;
   display: inline-block;
}
.home-text-content a:hover{
    transform: scale(1.1);
    background: var(--btn-color);
    border: 1px solid white;
}
.about{
    padding: 2rem 7%;
    background: var(--about-sec);
}
.main-about{
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    gap: 20px;
    
}
.about-content{
    flex: 1 1 45rem;
}
.about-inner-content{
    width: 100%;
    margin: 0 auto;
    padding-top: 3rem;
    padding-bottom: 3rem;
}
.about-content .about-inner-content img{
    width: 80%;
    margin-left: 100px;
}
.about-text-content{
    padding: 0 4rem;
}
.about-text-content h1{
    color: #e58f00;
    font-size: 40px;
    margin-bottom: 15px;
}
.about-text-content p{
    color: white;
    font-size: 1.5rem;
    line-height: 35px;
}
.quality{
    padding: 4rem 7%;
    background-image: linear-gradient(60.34deg, white 52.45%, var(--btn-color) 52.45%);
}
.main-quality{
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    gap: 15px;
}
.main-inner-quality{
    flex: 1 1 45rem;
}
.quality-content{
    padding: 0 4rem;
}
.quality-content h1{
    color: var(--btn-color);
    font-size: 40px;
    margin-bottom: 15px;
}
.quality-content p{
    color: var(--about-sec);
    font-size: 1.5rem;
    line-height: 30px;
}
.qulity-image{
    width: 100%;
}
.qulity-image img{
    width: 100%;
    object-fit: cover;
}
.gallery{
    padding: 4rem 7%;
    background: var(--about-sec);
}
.gallery h1{
    font-size: 30px;
    text-align: center;
    padding-bottom: 3rem;
    color: var(--btn-color);
    letter-spacing: 1px;
}
.main-gallery{
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 30px;
    flex-wrap: wrap;
  
}
.inner-gallery{
    flex: 1 1 300px;
    
}
.inner-gallery .gallery-image img{
    width: 100%;
}
.inner-gallery .gallery-image:hover img{
    transform: perspective(1000px) rotateX(-4.80deg) rotateY(-10.23deg) scale3d(1.05,1.05,1.05);
    clip-path: polygon(20% 0%, 80% 0%, 100% 20%, 100% 80%, 80% 100%, 20% 100%, 0% 80%, 0% 20%);
}
.enjoy-our-food{
    padding: 2rem 7%;
    background: url(images/enjoye.png);
    background-size: cover;
    background-position: center center;
    background-repeat: no-repeat;
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
}
.food-main-content{
    width: 40%;
    border: 4px solid white;
    padding: 2rem;
}
.food-main-content h1{
    color: white;
    font-size: 35px;
    text-align: center;
    padding: 1rem 0;
}
.food-main-content p{
    color: white;
    font-size: 1.5rem;
    text-align: center;
    padding: 1rem 0;
    line-height: 30px;
}
.our-menu-food{
    padding: 2rem 7%;
    background-color: var(--about-sec);
}
.our-menu-food h1{
    color: var(--btn-color);
    font-size: 45px;
    text-align: center;
    padding: 0.5rem 0;
}
.main-menu-food{
    margin-top: 2rem;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 20px;
    flex-wrap: wrap;
}
.inner-menu-food{
    flex: 1 1 300px;
}
.menu-food-content{
    width:100%;

}
.menu-food-content img{
    width: 100%;
}

.menu-food-text{
    padding: 2rem 2rem;
}
.menu-food-text h2{
    color: var(--btn-color);
    font-size: 30px;
}
.menu-food-text p{
    color:white;
    font-size:18px;
    margin: 2rem 0;
}
.menu-food-text p span{
    color: #e58f00;
    padding: 0.5rem 1.5rem;
    transition: 0.3s;
    cursor: pointer;
}
.menu-food-text p:hover span{
    border: 1px solid white;
    background: var(--btn-color);
    color: white;
    transform: scale(1.1);
}
.before{
    background-color: #1d1d23;
    padding: 2rem 0;
}
.before{
    width: 100%;
}
.before img{

    width: 100%;
    object-fit: cover;
}

.footer{
    background: #1d1d23;
    padding: 6rem 10rem;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
}
.main-footer{
    width: 100%;
    margin: 0 auto;
    text-align: center;
}
.main-footer img{
    width: 200px;
}
.footer-navbar{
    margin-top: 15px;
}
.footer-navbar a{
    color: #e58f00;
    font-size: 18px;
    margin: 1rem;
    padding: 1rem;
}

@media (max-width:767px) {
    .header{
        padding: 3rem;
    }
    .icons div{
        display: initial;
    }
    .navbar{
        position: absolute;
        width: 100%;
        height: 100vh;
        left: 0;
        top: 100%;
        background-color: var(--btn-color);
        clip-path: polygon(0 0, 100% 0, 100% 0, 0 0);


    }
    .navbar a{
        display: block;
        text-align: center;
        margin: 1rem;
        padding: 1rem;
    }

    /* home css desing */

    .home-text-content{
        padding: 0 2rem;
    }
    .main-home{
        padding: 2rem 0;
    }
    .home{
        padding-top: 100px;
        
    }
    .home-image img{
        transform: translate(0%, 0%);
    }
    .home-text-content{
        margin-top: 300px;
    }
    .about-content .about-inner-content img{
        width: 100%;
        margin: 0;
        padding: 1rem;
    }
    .quality-content{
        padding: 1rem 2rem;
    }
    .quality-content h1{
        color: var(--about-sec)
    }
    .food-main-content{
        width: 100%;
        border: 4px solid white;
        padding: 1rem;
    }

    .footer-navbar a{
        display: block;
       
    }

}
