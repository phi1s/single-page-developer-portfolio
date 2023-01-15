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
        <div class="image-profile" />
        <div class="hero-text">
          <h1>Nice to meet you! I'm <span>Adam Keyes</span>.</h1>
          <p>
            Based in the UK, I'm a front-end developer passionate about building
            accessible web apps that users love.
          </p>
        </div>
        <button>Contact me</button>
        <hr />
      </div>
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
      <hr />
      <div class="projects">
        <div class="inline">
          <h1>Projects</h1>
          <button>Contact me</button>
        </div>
        <ul>
          <li>
            <div class="thumbnail-project" id="tp1" />
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
        <h1>Contact</h1>
        <p>
          I would love to hear about your project and how I could help. Please
          fill in the form, and I'll get back to you as soon as possible.
        </p>
        <ContactForm />

        <hr class="hr-bottom" />
      </div>
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
    z-index: 1;
  }
  header > div {
    width: 100%;
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
  .projects > ul {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
  }
  .projects > ul > li {
    width: calc(50%-12px);
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
  }
}
@media screen and (min-width: 1200px) {
}
</style>
