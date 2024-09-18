<template>
  <div>

    <nav>
      <ul>
        <li><a href="#" @click.prevent="currentPage = 'home'">Inicio</a></li>
        <li><a href="#" @click.prevent="currentPage = 'jobs'">Trabajos</a></li>
        <li><a href="#" @click.prevent="currentPage = 'projects'">Proyectos</a></li>
        <li><a href="#" @click.prevent="currentPage = 'services'">Servicios</a></li>
        <li><a href="#" @click.prevent="currentPage = 'contact'">Contacto</a></li>
      </ul>
    </nav>

    <div v-if="currentPage === 'home'">
      <h1>Inicio</h1>
      <p>Bienvenido a nuestra página web, Nuestro equipo esta formado por Jesus Alejandro Granillo Erazo, David Ernesto Melara Rivas asi como tambien
        Jose Daniel Cortez Juarez y Miguel Alexis Arguera Ortiz.</p>
      <img src="https://png.pngtree.com/png-clipart/20210521/ourlarge/pngtree-home-button-ui-ux-png-image_3308787.jpg" alt="Imagen de inicio">
    </div>

    <div v-if="currentPage === 'jobs'">
      <h1>Trabajos</h1>
      <p>Aquí puedes ver algunos de los trabajos que hemos realizado para nuestros clientes.</p>
      <img src="https://images.unsplash.com/photo-1556761175-4b46a572b786?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=MnwzNjUyOXwwfDF8c2VhcmNofDI3fHxidXNpbmVzc3xlbnwwfHx8fDE2MDA3MjY5NDQ&ixlib=rb-1.2.1&q=80&w=1080" alt="Imagen de trabajos">
    </div>

    <div v-if="currentPage === 'projects'">
      <h1>Proyectos</h1>
      <p>Estos son algunos de los proyectos innovadores en los que estamos trabajando.</p>
      <img src="https://www.argentinaproduct.com/ckfinder/userfiles/files/blog/gestioct.jpg" alt="Imagen de proyectos">
    </div>

    <div v-if="currentPage === 'services'">
      <h1>Servicios</h1>
      <p>Ofrecemos una variedad de servicios de tecnología y consultoría creativa.</p>
      <img src="https://images.unsplash.com/photo-1542744095-fcf48d80b0fd?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=MnwzNjUyOXwwfDF8c2VhcmNofDE0fHxzZXJ2aWNlc3xlbnwwfHx8fDE2MDA3MjY5NDQ&ixlib=rb-1.2.1&q=80&w=1080" alt="Imagen de servicios">
    </div>

    <div v-if="currentPage === 'contact'">
      <h1>Contacto</h1>
      <p>Contáctanos para discutir cómo podemos colaborar en tu próximo proyecto.</p>
      <hr>
      <p>Puedes contactarnos por medio de WhatsApp asi como tambien por medio de Facebook como InnovaSoft</p>
      <img src="https://images.unsplash.com/photo-1494173853739-c21f58b16055?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=MnwzNjUyOXwwfDF8c2VhcmNofDI1fHxjb250YWN0fGVufDB8fHx8MTYwMDcyNjk0NA&ixlib=rb-1.2.1&q=80&w=1080" alt="Imagen de contacto">
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      currentPage: 'home', 
    };
  },
};
</script>

<style>

body {
  font-family: Arial, sans-serif;
  background-color: #f4f4f4;
  margin: 0;
  padding: 0;
}

nav {
  background-color: #333;
  padding: 10px;
}

nav ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: center;
}

nav ul li {
  margin: 0 15px;
}

nav ul li a {
  color: white;
  text-decoration: none;
  font-size: 18px;
}

nav ul li a:hover {
  text-decoration: underline;
}

h1 {
  text-align: center;
  margin-top: 20px;
}

p {
  text-align: center;
  font-size: 18px;
}

img {
  display: block;
  margin: 20px auto;
  max-width: 400px;
  width: 50%;
  height: auto;
}

</style>