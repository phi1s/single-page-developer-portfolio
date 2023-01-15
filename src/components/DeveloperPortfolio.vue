<template>
  <div>
    <div class="container">
      <header>
        <div>
          <h3 class="company">adamkeyes</h3>
          <div class="icons">
            <img src="../assets/images/icon-github.svg" alt="Icon GitHub" />
            <img
              src="../assets/images/icon-frontend-mentor.svg"
              alt="Icon Frontend Mentor"
            />
            <img src="../assets/images/icon-linkedin.svg" alt="Icon LinkedIn" />
            <img src="../assets/images/icon-twitter.svg" alt="Icon Twitter" />
          </div>
        </div>
      </header>
      <div class="background">
        <img
          src="../assets/images/pattern-circle.svg"
          alt="Pattern Circle"
          class="pattern-circle"
        />
        <div>
          <img
            src="../assets/images/pattern-rings.svg"
            alt="Pattern Rings"
            class="pattern-rings"
          />
          <img
            src="../assets/images/pattern-rings.svg"
            alt="Pattern Rings"
            class="pattern-rings"
          />
          <img
            src="../assets/images/pattern-rings.svg"
            alt="Pattern Rings"
            class="pattern-rings"
          />
        </div>
      </div>

      <div class="hero">
        <div class="image-profile">
          <img
            src="../assets/images/pattern-circle.svg"
            alt="Pattern Circle"
            class="pattern-circle-desktop"
          />
        </div>
        <div class="hero-text">
          <h1>Nice to meet you! I'm <span>Adam Keyes</span>.</h1>
          <p>
            Based in the UK, I'm a front-end developer passionate about building
            accessible web apps that users love.
          </p>
          <button>Contact me</button>
        </div>
      </div>
      <hr />
      <div class="stack">
        <ul>
          <li>
            <h2>HTML</h2>
            <p>4 Years Experience</p>
          </li>
          <li>
            <h2>CSS</h2>
            <p>4 Years Experience</p>
          </li>
          <li>
            <h2>Javascript</h2>
            <p>4 Years Experience</p>
          </li>
          <li>
            <h2>Accessiblility</h2>
            <p>4 Years Experience</p>
          </li>
          <li>
            <h2>React</h2>
            <p>3 Years Experience</p>
          </li>
          <li>
            <h2>Sass</h2>
            <p>3 Years Experience</p>
          </li>
        </ul>
      </div>
      <hr class="hr-projects" />
      <div class="projects">
        <div class="inline">
          <h1>Projects</h1>
          <button>Contact me</button>
        </div>
        <ul>
          <li>
            <div class="thumbnail-project" id="tp1" />
            <div class="overlay">
              <div class="learn-more-overlay">
                <button>View Project</button><br />
                <button>View Code</button>
              </div>
            </div>
            <h3>Design portfolio</h3>
            <ul>
              <li>HTML</li>
              <li>CSS</li>
            </ul>
            <div class="learn-more">
              <button>View Project</button><button>View Code</button>
            </div>
          </li>
          <li>
            <div class="thumbnail-project" id="tp2" />
            <div class="overlay">
              <div class="learn-more-overlay">
                <button>View Project</button><br />
                <button>View Code</button>
              </div>
            </div>
            <h3>E-learning landing page</h3>
            <ul>
              <li>HTML</li>
              <li>CSS</li>
            </ul>
            <div class="learn-more">
              <button>View Project</button><button>View Code</button>
            </div>
          </li>
          <li>
            <div class="thumbnail-project" id="tp3" />
            <div class="overlay">
              <div class="learn-more-overlay">
                <button>View Project</button><br />
                <button>View Code</button>
              </div>
            </div>
            <h3>Todo web app</h3>
            <ul>
              <li>HTML</li>
              <li>CSS</li>
              <li>Javascript</li>
            </ul>
            <div class="learn-more">
              <button>View Project</button><button>View Code</button>
            </div>
          </li>
          <li>
            <div class="thumbnail-project" id="tp4" />
            <div class="overlay">
              <div class="learn-more-overlay">
                <button>View Project</button><br />
                <button>View Code</button>
              </div>
            </div>
            <h3>Entertainment web app</h3>
            <ul>
              <li>HTML</li>
              <li>CSS</li>
              <li>Javascript</li>
            </ul>
            <div class="learn-more">
              <button>View Project</button><button>View Code</button>
            </div>
          </li>
          <li>
            <div class="thumbnail-project" id="tp5" />
            <div class="overlay">
              <div class="learn-more-overlay">
                <button>View Project</button><br />
                <button>View Code</button>
              </div>
            </div>
            <h3>Memory Game</h3>
            <ul>
              <li>HTML</li>
              <li>CSS</li>
              <li>Javascript</li>
            </ul>
            <div class="learn-more">
              <button>View Project</button><button>View Code</button>
            </div>
          </li>
          <li>
            <div class="thumbnail-project" id="tp6" />
            <div class="overlay">
              <div class="learn-more-overlay">
                <button>View Project</button><br />
                <button>View Code</button>
              </div>
            </div>
            <h3>Art gallery showcase</h3>
            <ul>
              <li>HTML</li>
              <li>CSS</li>
              <li>Javascript</li>
            </ul>
            <div class="learn-more">
              <button>View Project</button><button>View Code</button>
            </div>
          </li>
        </ul>
      </div>
    </div>
    <div class="contact">
      <div class="contact-text">
        <div>
          <h1>Contact</h1>
          <p>
            I would love to hear about your project and how I could help. Please
            fill in the form, and I'll get back to you as soon as possible.
          </p>
        </div>
        <ContactForm />
      </div>
      <hr class="hr-bottom" />
    </div>
    <footer>
      <div>
        <h3>adamkeyes</h3>
        <div class="icons">
          <img src="../assets/images/icon-github.svg" alt="Icon GitHub" />
          <img
            src="../assets/images/icon-frontend-mentor.svg"
            alt="Icon Frontend Mentor"
          />
          <img src="../assets/images/icon-linkedin.svg" alt="Icon LinkedIn" />
          <img src="../assets/images/icon-twitter.svg" alt="Icon Twitter" />
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
import ContactForm from "./ContactForm.vue";

export default {
  name: "DeveloperPortfolio",
  components: {
    ContactForm,
  },
  data() {
    return {
      msg: [],
      validEmail: {},
    };
  },
  methods: {
    validateAll() {
      this.validateEmail();
      return;
    },
    validateEmail() {
      /* eslint-disable */
      if (/^\w+([\.-]?\w+)*@\w+([\.-]?\w+)*(\.\w{2,3})+$/.test(this.email)) {
        this.validEmail = true;
      } else {
        this.validEmail = false;
      }
    },
  },
};
</script>

<style scoped>
.pattern-circle {
  position: absolute;
  top: 254px;
  right: -60px;
}

.pattern-circle-desktop {
  display: none;
}
.pattern-rings {
  position: absolute;
  width: 530px;
  height: 129px;
}
.pattern-rings:nth-child(1) {
  top: 124px;
  left: -350px;
}
.pattern-rings:nth-child(2) {
  top: 1515px;
  right: -350px;
}
.pattern-rings:nth-child(3) {
  bottom: 140px;
  left: -350px;
}

header {
  position: absolute;
  width: 100vw;
  display: flex;
  justify-content: center;
}

header > div {
  width: 154px;
  height: 72px;
}
.company {
  height: 32px;
}
.icons {
  height: 20px;
  display: flex;
  justify-content: space-between;
}
.image-profile {
  width: 174px;
  height: 383px;
  background-image: url("../assets/images/image-profile-mobile.webp");
  background-size: cover;
  background-repeat: no-repeat;
  margin: auto;
}
hr {
  margin: 80px 16px;
}
ul {
  padding: 0px;
  list-style-type: none;
}
.projects {
  text-align: start;
  margin: 0px 16px;
}
.inline {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.learn-more {
  display: flex;
  margin-top: 20px;
  margin-bottom: 40px;
}
.learn-more > button {
  margin-right: 30px;
}

.projects > ul > li > ul {
  display: flex;
  margin-bottom: 16px;
}
.projects > ul > li > ul > li {
  margin-right: 16px;
}
.thumbnail-project {
  width: 100%;
  height: 253px;
  background-size: cover;
  background-repeat: no-repeat;
}
#tp1 {
  background-image: url("../assets/images/thumbnail-project-1-small.webp");
}
#tp2 {
  background-image: url("../assets/images/thumbnail-project-2-small.webp");
}
#tp3 {
  background-image: url("../assets/images/thumbnail-project-3-small.webp");
}
#tp4 {
  background-image: url("../assets/images/thumbnail-project-4-small.webp");
}
#tp5 {
  background-image: url("../assets/images/thumbnail-project-5-small.webp");
}
#tp6 {
  background-image: url("../assets/images/thumbnail-project-6-small.webp");
}
.contact {
  background-color: #242424;
  padding: 60px 16px;
}

footer {
  background-color: #242424;
  width: 100%;
  margin-top: -100px;
  height: 160px;
  display: flex;
  justify-content: center;
}

@media screen and (min-width: 700px) {
  .container {
    margin: 30px;
  }
  header {
    width: calc(100vw - 60px);
    max-width: 1110px;
    z-index: 1;
  }
  header > div {
    width: 100%;
    max-width: 1110px;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .icons {
    height: 25px;
    width: 200px;
  }
  .image-profile {
    width: 322px;
    height: 600px;
    background-image: url("../assets/images/image-profile-tablet.webp");
    background-size: cover;
    background-repeat: no-repeat;
    position: absolute;
    top: 0;
    right: 0;
    z-index: 0;
  }
  .hero {
    width: 75%;
    padding-top: 150px;
  }
  .hero-text {
    position: relative;
  }
  .pattern-circle {
    z-index: 1;
    top: 470px;
  }
  .stack > ul {
    display: flex;
    flex-wrap: wrap;
  }
  .stack > ul > li {
    width: 50%;
  }
  .hr-projects {
    display: none;
  }
  .projects > ul {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
  }
  .projects > ul > li {
    width: 342px;
  }
  .contact {
    display: flex;
    justify-content: center;
    text-align: center;
  }
  .contact-text {
    max-width: 445px;
  }
  footer {
    padding: 100px 30px 0px 30px;
    width: calc(100vw - 60px);
  }
  footer > div {
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .hr-bottom {
    position: absolute;
    width: calc(100vw - 60px);
    left: 15px;
    bottom: 50px;
  }
}
@media screen and (min-width: 1200px) {
  .container {
    width: 1110px;
    margin-left: auto;
    margin-right: auto;
  }
  .header > div {
    margin: 0;
    max-width: 1110px;
  }
  .hero {
    width: 100%;
    display: flex;
    flex-direction: row-reverse;
    justify-content: space-between;
    padding-top: 0;
    margin-top: -30px;
  }
  .image-profile {
    width: 445px;
    height: 720px;
    background-image: url("../assets/images/image-profile-desktop.webp");
    background-size: cover;
    background-repeat: no-repeat;
    position: relative;
    margin: 0;
  }

  .hero-text {
    width: 445px;
    margin-top: 130px;
  }
  .hero-text > h1 {
    width: 800px;
  }
  .pattern-circle {
    display: none;
  }
  .pattern-circle-desktop {
    display: block;
    margin-top: 530px;
    margin-left: -60px;
  }
  .pattern-rings:nth-child(1) {
    top: 124px;
    left: -150px;
  }
  .icons {
    margin-right: 30px;
  }
  .projects > ul > li {
    width: 530px;
    margin-bottom: 60px;
  }
  .thumbnail-project {
    height: 400px;
  }
  .learn-more {
    display: none;
  }
  .overlay {
    position: absolute;
    margin-top: -400px;
    width: 530px;
    height: 400px;
    background-color: #000000;
    opacity: 0;
    z-index: 1;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .learn-more-overlay {
    display: block;
    text-align: center;
  }
  .learn-more-overlay > button {
    margin: 20px;
  }
  .overlay:hover {
    opacity: 0.75;
  }
  .contact-text {
    text-align: left;
    width: 1110px;
    max-width: 1110px;
    display: flex;
    justify-content: space-between;
  }
  .contact-text > div {
    width: 445px;
  }

  .hr-bottom {
    width: 1110px;
    left: auto;
  }

  footer > div {
    margin: 0;
    width: 1110px;
  }
}
</style>
