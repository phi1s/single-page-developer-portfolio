<template>
  <div>
    <header>
      <div class="container">
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
    </header>

    <div class="hero">
      <div class="image-profile" />
      <h1>Nice to meet you! I'm <span>Adam Keyes</span>.</h1>
      <p>
        Based in the UK, I'm a front-end developer passionate about building
        accessible web apps that users love.
      </p>

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
    <div class="contact">
      <h1>Contact</h1>
      <p>
        I would love to hear about your project and how I could help. Please
        fill in the form, and I'll get back to you as soon as possible.
      </p>

      <form>
        <input type="text" placeholder="Name" />
        <input type="email" placeholder="E-Mail" />
        <input type="text" placeholder="Message" />
        <button>Send message</button>
      </form>
      <hr />
    </div>
    <footer>
      <div class="container">
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
export default {
  name: "DeveloperPortfolio",
};
</script>

<style scoped>
header {
  position: absolute;
  width: 100vw;
  display: flex;
  justify-content: center;
}
.container {
  width: 154px;
  height: 72px;
}
.icons {
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
input {
  color: black;
  width: 100%;
  height: 43px;
  margin: 16px 0px;
  background-color: white;
  border: none;
}

footer {
  background-color: #242424;
  width: 100%;
  margin-top: -100px;
  height: 160px;
  display: flex;
  justify-content: center;
}
</style>
