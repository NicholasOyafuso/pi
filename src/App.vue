<script setup>
</script>

<template>
  <div class="page">
    <header>
      <div class="topo">
        <h2 class="logo">J&J</h2>
        <h3 class="data-header">June, 23rd 2026</h3>
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
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
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
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
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

/* ─── HEADER ─────────────────────────────────────────────── */
header {
  background: black;
  color: white;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px 40px;
  flex-wrap: wrap;
  gap: 12px;
}

.topo {
  display: flex;
  flex-direction: column;
}

.logo {
  font-weight: bold;
  font-size: clamp(1.8rem, 5vw, 3rem);
  line-height: 1;
}

.data-header {
  font-size: clamp(0.75rem, 2vw, 1rem);
  font-weight: normal;
}

nav {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
  justify-content: center;
}

nav a {
  color: white;
  text-decoration: none;
  font-size: clamp(11px, 1.5vw, 14px);
  white-space: nowrap;
}

/* ─── TÍTULO ─────────────────────────────────────────────── */
.titulo {
  text-align: center;
  padding: 40px 20px;
}

.titulo h1 {
  margin-top: 30px;
  margin-bottom: 30px;
  font-size: clamp(2rem, 8vw, 70px);
}

/* ─── HERO ───────────────────────────────────────────────── */
.hero {
  min-height: clamp(300px, 60vw, 900px);
  background: url("@/assets/imagem1.png") center/cover no-repeat;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 40px 20px;
}

.texto-hero {
  width: min(90%, 900px);
  font-size: clamp(1rem, 2.5vw, 2rem);
  text-align: center;
}

/* ─── CARTÕES ────────────────────────────────────────────── */
.cartoes {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: clamp(16px, 3vw, 40px);
  padding: clamp(20px, 5vw, 60px);
  justify-items: center;
}

.cartao {
  width: 100%;
  max-width: 400px;
  aspect-ratio: 3 / 5;
  background-size: cover;
  background-position: center;
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
  font-size: clamp(14px, 2vw, 22px);
  font-weight: bold;
  text-shadow: 2px 2px 10px black;
  text-decoration: underline;
}

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

/* ─── SEÇÃO LISTA ────────────────────────────────────────── */
.secao-lista {
  background: url("@/assets/image9.png") center/cover no-repeat;
  text-align: center;
  padding: clamp(60px, 12vw, 200px) clamp(16px, 5vw, 60px);
  color: white;
}

.secao-lista h2 {
  font-size: clamp(28px, 6vw, 67px);
  margin-bottom: 20px;
}

.secao-lista p {
  font-size: clamp(14px, 2vw, 25px);
  max-width: 800px;
  margin: 0 auto;
}

.secao-lista button {
  margin-top: 20px;
  padding: clamp(10px, 2vw, 15px) clamp(30px, 8vw, 100px);
  border: none;
  background: #6b4c7b;
  color: white;
  font-size: clamp(14px, 2vw, 20px);
  border-radius: 20px;
  cursor: pointer;
}

/* ─── CONVITE ────────────────────────────────────────────── */
.convite {
  background: #d99ad8;
  text-align: center;
  padding: clamp(40px, 8vw, 80px) 20px;
}

.convite h2 {
  font-size: clamp(18px, 3vw, 32px);
}

.convite button {
  margin-top: 20px;
  padding: 10px 50px;
  border: none;
  background: #ccc;
  font-size: clamp(14px, 2vw, 18px);
  cursor: pointer;
}

/* ─── FOOTER ────────────────────────────────────────────── */
footer {
  text-align: center;
  padding: 60px 20px;
  background: #ddd;
}

footer h1 {
  font-size: clamp(24px, 5vw, 40px);
  margin-bottom: 10px;
}

footer p {
  font-size: clamp(12px, 2vw, 16px);
}

/* ─── MOBILE  ──────────────────────────────────── */
@media (max-width: 480px) {
  header {
    flex-direction: column;
    align-items: center;
    text-align: center;
    padding: 16px 20px;
  }

  nav a {
    margin: 0 6px;
  }


  .cartoes {
    grid-template-columns: 1fr;
  }

  .cartao {
    max-width: 100%;
    aspect-ratio: 4 / 3;
  }

  .convite button {
    width: 80%;
    padding: 10px;
  }
}
</style>
