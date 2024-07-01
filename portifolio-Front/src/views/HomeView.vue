<script setup lang="ts">
import CardComponent from '@/components/CardComponent/CardComponent.vue'
import ProgressComponent from '@/components/ProgressComponent/ProgressComponent.vue'
import './Home.scss'

function clickProjects() {
  const projectsSection = document.getElementById('projects')
  if (projectsSection) {
    projectsSection.scrollIntoView({ behavior: 'smooth' })
  }
}

function clicktechnologies() {
  const techonologiesSection = document.getElementById('technologies')
  if (techonologiesSection) {
    techonologiesSection.scrollIntoView({ behavior: 'smooth' })
  }
}

function clickAboutMe() {
  const aboutMeSection = document.getElementById('aboutMe')
  if (aboutMeSection) {
    aboutMeSection.scrollIntoView({ behavior: 'smooth' })
  }
}
</script>

<template>
  <main class="container">
    <section class="SectionHome">
      <div class="contentHome">
        <ul class="listHome">
          <li class="liHome">
            <a class="textHome" @click="clickProjects"> Projetos</a>
          </li>
          <li class="liHome">
            <a class="textHome" @click="clicktechnologies">Tecnologias</a>
          </li>
          <li class="liHome">
            <a class="textHome" @click="clickAboutMe">Quem sou eu</a>
          </li>
        </ul>
        <div class="contentImgHome">
          <a href="https://github.com/gabrielolvrdev">
            <img class="imgGithub" src="/github.svg" />
          </a>
          <a href="https://www.linkedin.com/in/gabriel-oliveira-86b346255/">
            <img class="imgGithub" src="/Linkedin.png" />
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
              <button class="buttonBegin" @click="clickProjects">Ok!</button>
            </div>
          </div>
          <img class="imgDeveloper" src="/developer.png" />
        </div>
      </div>
    </section>
    <section class="sectionProjects">
      <div class="contentTitleProjects">
        <p class="titleSection" id="projects">Projetos</p>
      </div>
      <div class="contentProjects">
        <CardComponent
          title="BB Tranquilo"
          subtitle="Projeto feito para mamães para que possam tirar dúvidas sobre a gravidez e ter dicas sobre seus filhos."
        ></CardComponent>
        <CardComponent
          title="Landing Page"
          subtitle="Projeto de landing Pages feitas com componentes próprios para uso educacional"
        ></CardComponent>
        <CardComponent
          title="Conselho Biblico"
          subtitle="Conselhos Biblicos é um projeto voltado a pessoas que estão passando por uma situação e querem uma explicação biblica para isso"
        ></CardComponent>
        <CardComponent
          title="Pet Tranquilo"
          subtitle="Projeto voltado para tutores que querem dicas e tirar dúvidas sobre o dia a dia de seus Pets!"
        ></CardComponent>
      </div>
    </section>
    <section class="sectionTechnologies">
      <p class="titleSection" id="technologies">Tecnologias</p>
      <ProgressComponent
        class="styleProgress"
        :progress="99"
        titleProgress="HTML"
      ></ProgressComponent>
      <ProgressComponent
        class="styleProgress"
        :progress="95"
        titleProgress="CSS"
      ></ProgressComponent>
      <ProgressComponent
        class="styleProgress"
        :progress="70"
        titleProgress="JavaScript"
      ></ProgressComponent>
      <ProgressComponent
        class="styleProgress"
        :progress="65"
        titleProgress="Vuejs"
      ></ProgressComponent>
      <ProgressComponent
        class="styleProgress"
        :progress="40"
        titleProgress="RubyOnRails"
      ></ProgressComponent>
      <ProgressComponent
        class="styleProgress"
        :progress="65"
        titleProgress="Saas"
      ></ProgressComponent>
      <ProgressComponent
        class="styleProgress"
        :progress="70"
        titleProgress="TypeScript"
      ></ProgressComponent>
    </section>
    <section>
      <div class="contentSkills">
        <p class="titleSection">Tecnologias e Skills Adicionais</p>
        <ul>
          <li class="textList">GIT</li>
          <li class="textList">Scrum</li>
          <li class="textList">KANBAN</li>
          <li class="textList">Ingles</li>
        </ul>
      </div>
    </section>
    <section class="aboutMe" id="aboutMe">
      <div class="barAboutMe"></div>
      <p class="titleSection">Quem Sou Eu</p>
      <div>
        <div class="contentPerfil">
          <div class="contentPhotoPerfil">
            <img class="imagePerfil" src="../../public/perfil.jpeg" />
          </div>
          <div>
            <p class="textBegin">Gabriel Oliveira</p>
            <p class="textBegin">Desenvolvedor Front end</p>
          </div>
        </div>
        <div class="contentTextAboutMe">
          <p class="textBegin">
            Apaixonado por tecnologia desde muito cedo, concentrei meus estudos e forças para me
            posicionar no mercado de trabalho como alguém que sempre busca soluções que contribuam
            para o bem-estar de todos e também contribuir para uma melhor interação na equipe.
          </p>
        </div>
      </div>
      <div class="barAboutMe"></div>
    </section>
    <footer class="contentFooter">
      <p class="textBegin">Email: gogabriel35@gmail.com</p>
      <div class="contentImgHome">
        <a href="https://github.com/gabrielolvrdev">
          <img src="../../public/Linkedin.png" />
        </a>
        <a href="https://www.linkedin.com/in/gabriel-oliveira-86b346255/">
          <img src="../../public/github.svg" />
        </a>
      </div>
    </footer>
  </main>
</template>
