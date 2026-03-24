<script setup>
</script>

<template>
  <div class="page">
    <header>
      <div class="topo">
        <h2 class="logo">J&J</h2>
        <h3>June, 23rd 2026</h3>
      </div>

      <nav>
        <a href="#">HOME</a>
        <a href="#">OUR STORY</a>
        <a href="#">DETAILS</a>
        <a href="#">RSVP</a>
      </nav>
    </header>

    <section class="titulo">
      <h1>JENNY & JASON</h1>
    </section>

    <section class="hero">
      <div class="texto-hero">
        <p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod  tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim  veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea  commodo consequat. Duis aute irure dolor in reprehenderit in voluptate  velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint  occaecat cupidatat non proident, sunt in culpa qui officia deserunt  mollit anim id est laborum.
        </p>
      </div>
    </section>

    <section class="cartoes">
      <div class="cartao historia">
        <h2>OUR STORY</h2>
      </div>

      <div class="cartao detalhes">
        <h2>THE DETAILS</h2>
      </div>

      <div class="cartao rsvp">
        <h2>RSVP</h2>
      </div>

      <div class="cartao lista-presentes">
        <h2>REGISTRY</h2>
      </div>
    </section>

    <section class="secao-lista">
      <h2>REGISTRY</h2>

      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod  tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim  veniam, quis nostrud exercitation ullamco <br> laboris nisi ut aliquip ex ea  commodo consequat. Duis aute irure dolor in reprehenderit in voluptate  velit esse cillum dolore eu fugiat nulla pariatur. <br> Excepteur sint  occaecat cupidatat non proident, sunt in culpa qui officia deserunt  mollit anim id est laborum.
      </p>

      <button>GO TO REGISTRY</button>
    </section>

    <section class="convite">
      <h2>Get your invitation here</h2>
      <button>INVITATION</button>
    </section>

    <footer>
      <h1>J&J</h1>
      <p>SATURDAY,<br>SEPTEMBER 20, 2025</p>
    </footer>
  </div>
</template>

<style scoped>
*,
*::before,
*::after {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.page {
  font-family: Arial, sans-serif;
  background: #eaeaea;
  min-height: 100vh;
}

header {
  background: black;
  color: white;
  display: flex;
  justify-content: space-between;
  padding: 25px 40px;
  align-items: center;
}

nav a {
  color: white;
  margin-left: 25px;
  text-decoration: none;
  font-size: 14px;
}

.logo {
  font-weight: bold;
  font-size: 3rem;
}

.titulo {
  text-align: center;
  padding: 40px;
}

.titulo h1 {
  margin-top: 30px;
  margin-bottom:30px;
  font-size: 70px;
}

.hero {
  height: 900px;
  background: url("@/assets/imagem1.png") center/cover no-repeat;
  display: flex;
  justify-content: center;
  align-items: center;
}

.texto-hero {
  width: 1500px;
  font-size:2rem;
  text-align: center;
  padding: 20px;
}

.cartoes {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 40px;
  padding: 60px;
  justify-items: center;
}

.cartao {
  width: 300px;
  height: 500px;
  background-size: cover;
  background-position: center;
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
  font-size: 22px;
  font-weight: bold;
  text-shadow: 2px 2px 10px black;
  text-decoration: underline;}

.historia {
  background-image: url("@/assets/image1.png");
}

.detalhes {
  background-image: url("@/assets/image2.png");
}

.rsvp {
  background-image: url("@/assets/image7.png");
}

.lista-presentes {
  background-image: url("@/assets/image5.png");
}

.secao-lista {
  background: url("@/assets/image9.png") center/cover no-repeat;
  text-align: center;
  padding: 200px 20px;
  color: white;
}
.secao-lista p {
  font-size:25px;
}
.secao-lista h2 {
  font-size:67px;
  margin-bottom:20px;
}


.secao-lista button {
  margin-top: 20px;
  padding: 15px 100px;
  border: none;
  background: #6b4c7b;
  color: white;
  font-size:20px;
  border-radius: 20px;
}

.convite {
  background: #d99ad8;
  text-align: center;
  padding: 80px;
}

.convite button {
  margin-top: 20px;
  padding: 10px 50px;
  border: none;
  background: #ccc;
  font-size: 18px;
}

footer {
  text-align: center;
  padding: 60px;
  background: #ddd;
}

footer h1 {
  font-size: 40px;
  margin-bottom: 10px;
}

@media (max-width: 768px) {
  header {
    flex-direction: column;
    gap: 10px;
    text-align: center;
  }

  nav a {
    margin: 0 10px;
    font-size: 12px;
  }

  .titulo h1 {
    font-size: 35px;
  }

  .hero {
    height: 300px;
    padding: 20px;
  }

  .texto-hero {
    width: 90%;
    font-size: 14px;
  }

  .cartoes {
    grid-template-columns: 1fr;
    padding: 30px;
    gap: 25px;
  }

  .cartao {
    width: 100%;
    max-width: 300px;
    height: 300px;
  }

  .secao-lista {
    padding: 60px 20px;
  }

  .secao-lista h2 {
    font-size: 28px;
  }

  .secao-lista p {
    font-size: 14px;
  }

  .convite {
    padding: 60px 20px;
  }

  .convite h2 {
    font-size: 24px;
  }

  .convite button {
    width: 80%;
  }

  footer h1 {
    font-size: 30px;
  }

  footer p {
    font-size: 14px;
  }
}
</style>
