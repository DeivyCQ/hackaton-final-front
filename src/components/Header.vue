<template>
   <header>
      <div class="header">
         <nav>
            <div class="menu">
               <img src="../assets/Pachaqtec-logo.jpg" alt="" class="menu-logo" />
               <div class="menu-list">
                  <ul>
                     <li class="menu-item"><a href="#" class="menu-link"></a>Home</li>
                     <li class="menu-item"><a href="#" class="menu-link"></a>About</li>
                     <li class="menu-item"><a href="#" class="menu-link"></a>Contacts</li>
                     <li class="menu-item"><a href="#" class="menu-link"></a>Services</li>
                     <li class="menu-item"><a href="#" class="menu-link"></a>More</li>
                  </ul>
               </div>
               <div class="menu-rigth">
                  <a href=""><i class="fas fa-shopping-cart"></i></a>
                  <a href=""><i class="fas fa-bars"></i></a>
               </div>
            </div>
         </nav>
         <section class="section-banner">
            <div class="banner">
               <div class="banner-text">
                  <h1>Explota todo tu potencial tecnológico!</h1>
                  <p>Con nuestros programas de especialización</p>
               </div>
               <div class="formulario">
                  <form>
                     <p>Postula y obtén un 10% de descuento ne el programa</p>
                     <div>
                        <input type="text" placeholder="NOMBRE" />
                     </div>
                     <div>
                        <input type="text" placeholder="CELULAR" />
                     </div>
                     <div>
                        <input type="text" placeholder="CORREO ELECTRONICO" />
                     </div>
                     <div>
                        <input type="text" placeholder="PROGRAMA" />
                     </div>
                     <div class="check">
                        <input type="checkbox" value="privacidad" id="privacidad" />
                        <label for="privacidad">Acepto las Políticas de privacidad.</label>
                     </div>
                     <input type="submit" value="Quiero postular" class="btn" />
                  </form>
               </div>
            </div>
         </section>
      </div>
      <section class="section-grupos">
         <div class="grupos">
            <img src="../assets/Intercorp.svg" alt="" />
            <img src="../assets/idat.png" alt="" />
            <img src="../assets/zegel.png" alt="" />
         </div>
      </section>
   </header>
</template>

<script>
export default {
   name: 'Header',
};
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@100;300;400;500&display=swap');

* {
   box-sizing: border-box;
   margin: 0;
   padding: 0;
}
body {
   font-family: 'Roboto', sans-serif;
}
a {
   text-decoration: none;
}
li {
   list-style: none;
}
header {
   min-height: 100vh;
}
.header {
   background-color: #5640ff;
}
/* seccion menu */
.menu {
   max-width: 90%;
   height: 70px;
   margin-left: auto;
   margin-right: auto;
   display: flex;
   justify-content: space-between;
   align-items: center;
}
.menu-logo {
   width: 200px;
}
.menu-list ul {
   display: flex;
   justify-content: space-between;
   align-items: center;
}
.menu-item {
   margin: 0 15px;
   color: white;
}
.menu-rigth a {
   margin: 0 10px;
   color: white;
}
/* banner */
.banner {
   max-width: 90%;
   margin-right: auto;
   margin-left: auto;
   display: flex;
   align-items: center;
   margin-top: 20px;
}
.banner-text {
   max-width: 70%;
   color: white;
   margin-top: 100px;
   text-align: left;
   margin-bottom: 100px;
}
.banner h1 {
   font-size: 3rem;
}
.banner p {
   margin-top: 40px;
   font-size: 1.2rem;
}
/* formulario */
.formulario {
   min-width: 280px;
   background-color: white;
   position: relative;
   top: 100px;
   border-radius: 5px;
}
.formulario form {
   padding: 8px;
   margin-right: auto;
   margin-left: auto;
}
.formulario div {
   margin-bottom: 15px;
}
.formulario p {
   font-size: 1rem;
   font-weight: bold;
   margin-bottom: 15px;
}
.formulario input {
   width: 85%;
   padding: 15px 5px;
   border: 1px solid black;
   border-radius: 3px;
}
.check input {
   width: auto;
}
.check label {
   font-size: 0.8rem;
   font-weight: bold;
}
.btn {
   background-color: #5640ff;
   color: white;
}
/* seccion grupos */
.grupos {
   max-width: 90%;
   margin-top: 30px;
   margin-left: auto;
   margin-right: auto;
   display: flex;
   justify-content: right;
   align-items: center;
}
.grupos img {
   width: 100px;
}

@media screen and (max-width: 670px) {
   .formulario {
      display: none;
   }
}
@media screen and (max-width: 800px) {
   /* /* .menu-list {
      /* display: none; 

   }  */
   .menu-list ul {
      position: absolute;
      flex-direction: column;
      justify-content: space-between;
      height: 300px;
      background-color: grey;
   }
}
</style>
