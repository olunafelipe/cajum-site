<template>
    <section id="quem-somos" class="quem-somos-section">
      <img src="/quem-somos-title.png" alt="Quem Somos" class="titulo-img" />
      <div class="conteudo">
        <img src="/quem-somos-left-image.png" alt="Imagem Esquerda" class="imagem-esquerda" />
        <div class="texto">
          <p>
            A Casa de Artes da Juventude Metodista (CAJUM) nasceu em 2025 com o propósito de proclamar o evangelho por meio das artes. Acreditamos que a criatividade é uma poderosa ferramenta para tocar corações e transformar vidas, levando a mensagem de Cristo de forma autêntica e impactante.
          </p>
          <p>
            Nossos ministérios de Música, Dança, Teatro, Circo, Evangelismo, Intercessão e Comunicação se unem para expressar a fé através da arte. Cada apresentação, ensaio e projeto são oportunidades de inspirar pessoas e espalhar o amor de Deus ao mundo.
          </p>
        </div>
      </div>
      <div class="letreiro-container">
      <div class="letreiro-texto">
        <span>* VEM PRA CAJUM * VEM PRA CAJUM * VEM PRA CAJUM * VEM PRA CAJUM * VEM PRA CAJUM * VEM PRA CAJUM * VEM PRA CAJUM * VEM PRA CAJUM *</span>
        <span>* VEM PRA CAJUM * VEM PRA CAJUM * VEM PRA CAJUM * VEM PRA CAJUM * VEM PRA CAJUM * VEM PRA CAJUM * VEM PRA CAJUM * VEM PRA CAJUM *</span>
      </div>
    </div>
    </section>
  </template>
  
  <style scoped>
  @import url('https://fonts.googleapis.com/css2?family=Rubik:wght@500&display=swap');
  .quem-somos-section {
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    padding: 50px 20px;
    text-align: center;
  }
  
  .titulo-img {
    width: 30%;
    max-width: 600px;
    margin-bottom: 20px;
    margin-top: -150px;
  }
  
  .conteudo {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 40px;
    max-width: 1200px;
    width: 100%;
  }
  
  .imagem-esquerda {
    width: 45%;
    max-width: 500px;
    margin-top: 20px;
  }
  
  .texto {
    width: 45%;
    font-size: 1.2rem;
    line-height: 1.6;
    text-align: center;
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif
  }
  
  .texto p {
    margin-bottom: 15px;
  }

.letreiro-container {
  width: 100%;
  background-color: #621EAA;
  overflow: hidden;
  white-space: nowrap;
  position: relative;
  padding: 25px 0;
  padding-top: 20px;
  display: flex;
  align-items: center;
}

.letreiro-texto {
  display: flex;
  font-size: 3.0rem;
  font-weight: bold;
  color: #FFC552;
  text-transform: uppercase;
  font-family: 'Rubik', sans-serif;
  width: max-content;
  animation: marquee 15s linear infinite;
}

.letreiro-texto span {
  display: inline-block;
  padding-right: 1rem;
  white-space: nowrap;
}

@keyframes marquee {
  from {
    transform: translateX(0);
  }
  to {
    transform: translateX(-50%);
  }
}
  </style>
  