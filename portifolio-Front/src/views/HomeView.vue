<script setup lang="ts">
import './Home.scss'
</script>

<template>
  <main class="container">
    <section class="SectionHome">
      <div class="contentHome">
        <ul class="listHome">
          <li class="liHome">
            <a class="textHome">Portifólio</a>
          </li>
          <li class="liHome">
            <a class="textHome"> Projects</a>
          </li>
          <li class="liHome">
            <a class="textHome">Technologies</a>
          </li>
          <li class="liHome">
            <a class="textHome">About me</a>
          </li>
        </ul>
        <div class="contentImgHome">
          <a href="https://github.com/gabrielolvrdev">
            <img src="/public/github.svg" />
          </a>
          <a href="https://www.linkedin.com/in/gabriel-oliveira-86b346255/">
            <img src="/public/Linkedin.png" />
          </a>
        </div>
      </div>
    </section>
    <section class="sectionBegin">
      <div class="contentBegin">
        <h1 class="titleSection">Bem vindo ao meu Pórtifólio!</h1>
        <div class="contentParagraphBegin">
          <div class="paragraphBegin">
            <p class="textBegin">
              Neste portfólio, você encontrará uma seleção de projetos que destacam minha habilidade
              em design, codificação e resolução de problemas. Cada projeto reflete meu compromisso
              com a excelência e a inovação no desenvolvimento web. Obrigado por visitar e sinta-se
              à vontade para entrar em contato!
            </p>
            <div class="contentButtonBegin">
              <button class="buttonBegin">lets bora</button>
            </div>
          </div>
          <img class="imgDeveloper" src="/public/developer.png" />
        </div>
      </div>
    </section>
    <section class="sectionProjects">
      <div>
        <p class="titleSection">Projects</p>
      </div>
      <div class="contentProjects">
        <div></div>
      </div>
    </section>
  </main>
</template>
