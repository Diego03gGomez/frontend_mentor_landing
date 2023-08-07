<template lang="">
    <div>
     
<header>
<div class="cont_header">
    <i v-on:click="desplegar()" class="fa-solid fa-bars menu"></i>

<div class="menu_oculto ">
<a href="">Home</a>
<a href="">About</a>
<a href="">Contact</a>
<a href="">Blog</a>
<a href="">Carrers</a>
</div>



<h1><img src="https://easybankapp-eight.vercel.app/static/media/logo.4d7cebc59950e27d6f943b4c63129d81.svg" alt=""></h1>

<nav>
    <ul>
        <a href="">Home</a>
        <a href="">About</a>
        <a href="">Contact</a>
        <a href="">Blog</a>
        <a href="">Carrers</a>
    </ul>
</nav>


<a  class="invitar1" href="">Request invite</a>



</div>


</header>




<div data-aos="fade-down"     id="fondo1">

<div class="cont_todo">
    <div  class="cont1_fondo1">
<h1>Next generation <br>
digital banking</h1>
<p>Take your financial life online. Your Easybank account <br>
wil be a one-shop for spending, saving <br>
budgeting, investing, and more.</p>

<a  class="invitar" href="">Request invite</a>



</div>


<div  class="cont2_fondo1">

    <img src="https://leonidasesteban.github.io/easybank-learning-sass/static/images/image-mockups.png" alt="">

</div>

</div>






</div>



<div id="fondo2">
    
<div  class="titulo_fondo2">
<h1>Why choose Easybank?</h1>
<p>We leverange Open Banking to turn your bank account into your financial hub. <br>
Control your finances like never before</p>

</div>

<div class="cont_fondo2">

<div  data-aos="fade-down" v-for="(e, index) in info_card2" :key="index" class="card_f2">
<div class="logos">
    <img :src="e.imagen1" alt="">
</div>
<h2>{{e.titulo}}</h2>

<p>{{e.descripcion}}</p>
</div>



</div>




}</div>



<div id="fondo3">

    <div  data-aos="fade-down" class="titulo_fondo3">
        <h1>Latest Article</h1>
    </div>

<div class="cont_fondo3">

<div  data-aos="fade-down" v-for="(e, index) in arrayarticulos" :key="index" class="card_articulo">
<div class="img_articulo">
    <img :src="e.img_articulo" alt="">
</div>
<p>By {{e.autor_articulo}}  </p>
<h2>{{e.titulo_art}}</h2>
<p>{{e.des_art}}</p>

</div>


</div>



</div>




<footer>

<div class="cont_footer">

    <div class="columna1">
<h2><img src="https://easybankapp-eight.vercel.app/static/media/logo.4d7cebc59950e27d6f943b4c63129d81.svg" alt=""></h2>
<div class="redes">
    <a href=""><i class="fa-brands fa-facebook"></i></a>
    <a href=""><i class="fa-brands fa-youtube"></i></a>
    <a href=""><i class="fa-brands fa-twitter"></i></a>
    <a href=""><i class="fa-brands fa-pinterest"></i></a>
    <a href=""><i class="fa-brands fa-instagram"></i></a>
</div>

    </div>

    <div class="columna2">
<a href="">About Us</a>
<a href="">Contact</a>
<a href="">Blog</a>
    </div>


    <div class="columna3">
        <a href="">Careers</a>
        <a href="">Support</a>
        <a href="">Privacy Policy</a>
    </div>

<div class="columna4">
<a  class="invitar" href="">Rquest invite</a>
<p>@Easy banl. All Rights Reserved</p>

</div>


</div>

</footer>







    </div>
</template>
<script>
export default {

data() {
    return {
        info_card2: [
{imagen1:"https://easybankapp-eight.vercel.app/static/media/icon-online.b0622b15741418e9efe3805d1b2ac26b.svg", titulo:"Online Banking", descripcion: "Our modern web and mobile applications allow you to keep track of your finances wherever you are in the world" },
{imagen1:"https://easybankapp-eight.vercel.app/static/media/icon-budgeting.ad7169975ea1eda87072ea0325a8204a.svg", titulo:"Simple Budgeting", descripcion: "See exaclty where your money goes each month. Receive notification when you re close to hitting your limits" },
{imagen1:"https://easybankapp-eight.vercel.app/static/media/icon-onboarding.d74aed6429619336a30e42334d6eb432.svg", titulo:"Fast Onboarding", descripcion: "We dont do branches. Open your account in minutes online and start talking control of your finances right away" },
{imagen1:"https://easybankapp-eight.vercel.app/static/media/icon-api.74c8ad1751bbd1e7f545e458f9306885.svg", titulo:"Open API", descripcion: "Manage your savings, investments, pension and much more from one account. Tracking your money has never benn easier." },        
],
arrayarticulos: [
    {img_articulo: "https://images.squarespace-cdn.com/content/v1/5ea1a27dc644452fecd2e9b5/1593721163843-U2EMKZ7YNSSFYV3LCKR4/image-asset.jpeg", autor_articulo: "Clarence Robbinson", titulo_art: "Receive money in any currency with no fees", des_art: "The worlds is getting smaller and we re becoming more mobile. So why should you be forced to only receive money in a single..."}, 
    {img_articulo: "https://images.squarespace-cdn.com/content/v1/5fc75bdeabffab30daabad85/1606988592695-NDWLUGVKQAY6CQWVQ68D/jay-wennington-N_Y88TWmGwA-unsplash.jpg", autor_articulo: "Wilson Hutton", titulo_art: "Treat yourself without worryng about money", des_art: "Our simple budgeting feature allows you to separate out your spending and set realistic limits each month. That means you.."},


    {img_articulo: "https://th.bing.com/th/id/OIP.UAHkyYE61Dv3-lFWsPTxuwHaFj?pid=ImgDet&w=1600&h=1200&rs=1" , autor_articulo: "Wilson Hutton", titulo_art: "Take your Easybank card wherever you go", des_art: "We want you to enjoy your travels. This is why we don t charge any fees on purchases while you re abroad. We all even show you.."},

    {img_articulo: "https://images.unsplash.com/photo-1513151233558-d860c5398176?ixlib=rb-1.2.1&q=80&fm=jpg&crop=entropy&cs=tinysrgb&w=400&fit=max&ixid=eyJhcHBfaWQiOjE4MjY3M30" , autor_articulo: "Clarence Robbinson", titulo_art: "Our invite-only Beta accounts are now live!", des_art: "After a lot of hard work by the whole team, we re excited to launch our closed beta. Its seasy to request an invite throug the site"},

]
 ,

    }
},

methods: {
    desplegar(){

        let menu = document.querySelector(".menu_oculto");
        menu.classList.toggle("desplazar");
        
    }
},
mounted () {
    AOS.init();
},

    
}
</script>
<style lang="">
    
</style>