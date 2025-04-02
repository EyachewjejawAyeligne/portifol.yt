

*{
    margin: 0%;
    padding: 0%;
    box-sizing: border-box;
    font-family: poppis,sans-serif;
}
/*body{
    background-color:#1f242d;
}*/

a {
    color: rgb(212, 210, 233);
    text-decoration: none;
}

.navbar{
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    padding: 25px 9%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    z-index: 100;
    visibility: hidden;
    opacity: 0;
    animation:show-content 1.5s linear forwards;
    animation-delay: 1.2s;

}
@keyframes show-content{
    100% {
    visibility:visible;
    opacity:1;
}
}
.navbar logo{
    font-size: 30px;
    font-weight: 700;

}
.navbar ul{
    display: flex;
}
.navbar ul li {
    list-style: none;
    margin-left: 35px;


}
.navbar ul li a{
    font-size: 20px;
    font-weight: 500;
    transition: 0.5s;

}
.navbar ul li :hover{
    color: rgb(42, 182, 166);


}
.home{
    display: flex;
    align-items: center;
    gap: 50px;
    height: 100vh;
    padding: 60px 9% 0;
    color: aliceblue;
    visibility: hidden;
    opacity: 0;
    animation:show-content 1.5s linear forwards;
    animation-delay: 1.6s;

}
.home-info h1{
    font-size: 55px;

}

.home-info h2{
    display: inline-block;
    font-size: 32px;
    margin-top: -10px;

}
.home-info h2 span {
    position: relative;
    display:inline-block;
    color: transparent;
    -webkit-text-stroke: .7px #7cf03d;
    animation:display-text 16s linear infinite;
    animation-delay: calc(-4s * var(--i));
}
@keyframes display-text {
    25%,
100% 

{
     display: none;

     }
      }
      .home-info h2 span::before {
    content: attr(data-text);
    position:absolute;
    width:0;
    border-right:2px solid  #7cf03d;
    color:green;
    white-space: nowrap;
    overflow: hidden;
    animation: fill-text 4s linear infinite;


     }

@keyframes fill-text {
    10%,100%{
        width: 0;
    }
    70%,
    90%
    {
        width: 100%;
    }
}

.home-info p{
    font-size: 16px;
    margin: 10px 0 25px;

}
.home-info .btn-sci {
    display: flex;
    align-items: center;
}

.btn {
    display: inline-block;
    padding: 10px 30px;
    background: rgb(25, 225, 109);
    border:2px solid green;
    border-radius: 40px;
    box-shadow: 0 0 10px green;
    font-size: 16px;
    color: black;
    font-weight: 600;
    transition: .5s;


}
.btn:hover{
    background: transparent;
    color: rgb(179, 223, 20);
    box-shadow: none;

}
.home-info .btn-sci .sci {
    margin-left: 20px;
}
.home-info .btn-sci .sci a {
    display: inline-flex;
    padding: 8px;
    border: 2px solid green;
    border-radius: 50px;
    font-size: 20px;
    color: green;
    margin: 0 8px;
    transition: 0.5s;
}
.home-info .btn-sci .sci a:hover {
    background: greenyellow;
    color:black;
    box-shadow: 0 0 10px  greenyellow;

}

.home-img .img-box {
    position: relative;
    width: 32vw;
    height: 32vw;
    border-radius: 50%;
    padding: 5px;
    display: flex;
    justify-content: center;
    align-items: center;
    overflow: hidden;
}

.home-img .img-box::before,
.home-img .img-box::after {
    content: '';
    position: absolute;
    width: 700px;
    height: 500px;
    background: conic-gradient(transparent,transparent,
    transparent,rgb(92, 248, 92));
    transform: rotate(0deg);
    animation: rotate-border 10s linear infinite;

}
.home-img .img-box::after{
    animation-delay: -5s;
}
@keyframes rotate-border {
    100%{transform: rotate(360deg);

    }

}
.home-img .img-box .img-item {
    position: relative;
    width: 100%;
    height: 100%;
    background: #1f242d;
    border-radius: 50%;
    border:.1% solid #1f242d;
    display: flex;
    justify-content: center;
    z-index: 1;
    overflow: hidden;


}
.home-img  .mg-box .img-item img{
    position: absolute;
    top: 30px;
    display:block;
    width: 85%;
    object-fit: cover;
    mix-blend-mode:lighten;
}
.bars-animation {
    position: absolute;
    width: 100%;
    height: 100%;
    display: flex;
    z-index: -1;

}
.bars-animation .bar{
    width: 100%;
    height: 100%;
    background: #1f242d;
    /*border: 2px solid blue;*/
    transform: translateY(-100%);
    animation: show-bars .5s ease-in-out forwards;
    animation-delay: calc(.1s*var(--i));

}
@keyframes show-bars {
    100%{
        transform: translateY(0%);

    }
}
.logo {
    font-size: 24px;

}
<style>*{
    margin: 0%;
    padding: 0%;
    box-sizing: border-box;
    font-family: poppis,sans-serif;
}
/*body{
    background-color:#1f242d;
}*/

a {
    color: rgb(212, 210, 233);
    text-decoration: none;
}

.navbar{
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    padding: 25px 9%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    z-index: 100;
    visibility: hidden;
    opacity: 0;
    animation:show-content 1.5s linear forwards;
    animation-delay: 1.2s;

}
@keyframes show-content{
    100% {
    visibility:visible;
    opacity:1;
}
}
.navbar logo{
    font-size: 30px;
    font-weight: 700;

}
.navbar ul{
    display: flex;
}
.navbar ul li {
    list-style: none;
    margin-left: 35px;


}
.navbar ul li a{
    font-size: 20px;
    font-weight: 500;
    transition: 0.5s;

}
.navbar ul li :hover{
    color: rgb(42, 182, 166);


}
.home{
    display: flex;
    align-items: center;
    gap: 50px;
    height: 100vh;
    padding: 60px 9% 0;
    color: aliceblue;
    visibility: hidden;
    opacity: 0;
    animation:show-content 1.5s linear forwards;
    animation-delay: 1.6s;

}
.home-info h1{
    font-size: 55px;

}

.home-info h2{
    display: inline-block;
    font-size: 32px;
    margin-top: -10px;

}
.home-info h2 span {
    position: relative;
    display:inline-block;
    color: transparent;
    -webkit-text-stroke: .7px #7cf03d;
    animation:display-text 16s linear infinite;
    animation-delay: calc(-4s * var(--i));
}
@keyframes display-text {
    25%,
100% 

{
     display: none;

     }
      }
      .home-info h2 span::before {
    content: attr(data-text);
    position:absolute;
    width:0;
    border-right:2px solid  #7cf03d;
    color:green;
    white-space: nowrap;
    overflow: hidden;
    animation: fill-text 4s linear infinite;


     }

@keyframes fill-text {
    10%,100%{
        width: 0;
    }
    70%,
    90%
    {
        width: 100%;
    }
}

.home-info p{
    font-size: 16px;
    margin: 10px 0 25px;

}
.home-info .btn-sci {
    display: flex;
    align-items: center;
}

.btn {
    display: inline-block;
    padding: 10px 30px;
    background: rgb(25, 225, 109);
    border:2px solid green;
    border-radius: 40px;
    box-shadow: 0 0 10px green;
    font-size: 16px;
    color: black;
    font-weight: 600;
    transition: .5s;


}
.btn:hover{
    background: transparent;
    color: rgb(179, 223, 20);
    box-shadow: none;

}
.home-info .btn-sci .sci {
    margin-left: 20px;
}
.home-info .btn-sci .sci a {
    display: inline-flex;
    padding: 8px;
    border: 2px solid green;
    border-radius: 50px;
    font-size: 20px;
    color: green;
    margin: 0 8px;
    transition: 0.5s;
}
.home-info .btn-sci .sci a:hover {
    background: greenyellow;
    color:black;
    box-shadow: 0 0 10px  greenyellow;

}

.home-img .img-box {
    position: relative;
    width: 32vw;
    height: 32vw;
    border-radius: 50%;
    padding: 5px;
    display: flex;
    justify-content: center;
    align-items: center;
    overflow: hidden;
}

.home-img .img-box::before,
.home-img .img-box::after {
    content: '';
    position: absolute;
    width: 700px;
    height: 500px;
    background: conic-gradient(transparent,transparent,
    transparent,rgb(92, 248, 92));
    transform: rotate(0deg);
    animation: rotate-border 10s linear infinite;

}
.home-img .img-box::after{
    animation-delay: -5s;
}
@keyframes rotate-border {
    100%{transform: rotate(360deg);

    }

}
.home-img .img-box .img-item {
    position: relative;
    width: 100%;
    height: 100%;
    background: #1f242d;
    border-radius: 50%;
    border:.1% solid #1f242d;
    display: flex;
    justify-content: center;
    z-index: 1;
    overflow: hidden;


}
.home-img  .mg-box .img-item img{
    position: absolute;
    top: 30px;
    display:block;
    width: 85%;
    object-fit: cover;
    mix-blend-mode:lighten;
}
.bars-animation {
    position: absolute;
    width: 100%;
    height: 100%;
    display: flex;
    z-index: -1;

}
.bars-animation .bar{
    width: 100%;
    height: 100%;
    background: #1f242d;
    /*border: 2px solid blue;*/
    transform: translateY(-100%);
    animation: show-bars .5s ease-in-out forwards;
    animation-delay: calc(.1s*var(--i));

}
@keyframes show-bars {
    100%{
        transform: translateY(0%);

    }
}
.logo {
    font-size: 24px;

}
</style>
