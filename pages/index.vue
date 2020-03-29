<template>
  <div>
    <div class="blob">
      <svg
        xmlns:xlink="http://www.w3.org/1999/xlink"
        version="1.1"
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 310 350"
      >
        <path
          d="M156.4,339.5c31.8-2.5,59.4-26.8,80.2-48.5c28.3-29.5,40.5-47,56.1-85.1c14-34.3,20.7-75.6,2.3-111  c-18.1-34.8-55.7-58-90.4-72.3c-11.7-4.8-24.1-8.8-36.8-11.5l-0.9-0.9l-0.6,0.6c-27.7-5.8-56.6-6-82.4,3c-38.8,13.6-64,48.8-66.8,90.3c-3,43.9,17.8,88.3,33.7,128.8c5.3,13.5,10.4,27.1,14.9,40.9C77.5,309.9,111,343,156.4,339.5z"
        />
      </svg>
    </div>

    <div class="maindiv">
      <h1>
        Hi, I'm
        <br />Anugeeth !
      </h1>
      <div class="card-social">
        <p class="text">I Code 👨‍💻</p>
        <div class="icons">
          <a href="https://github.com/Anugeeth/">
            <font-awesome-icon :icon="['fab', 'github']" />
          </a>
          <a href="https://www.linkedin.com/in/anugeeth2/">
            <font-awesome-icon :icon="['fab', 'linkedin']" />
          </a>
          <a href="https://t.me/anugeeth2/">
            <font-awesome-icon :icon="['fab', 'telegram']" />
          </a>
         
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  components: {},

  head() {
    return {
      title: "Home"
    };
  }
};
</script>

<style>
/* @import url("https://fonts.googleapis.com/css?family=Poppins:700"); */
body {
  margin: 0;
  padding: 0;
  background: #ffb1a4;
  overflow: hidden;
}

.maindiv {
  width: 100vw;
  height: 100vh;
  position: relative;
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  overflow: hidden;
}

h1 {
  color: white;
  font-size: 15vmin;
  line-height: 1;
  font-weight: bold;
  letter-spacing: 2px;
  font-family: "Poppins", sans-serif;
  /* text-transform: uppercase; */
  padding-left: 40px;
}

.blob {
  position: absolute;
  top: 0;
  left: 0;
  fill: #023f92;
  width: 50vmax;
  z-index: -1;
  animation: move 10s ease-in-out infinite;
  transform-origin: 50% 50%;
}

.card-social {
  background-color: white;
  font-family: "Poppins", sans-serif;
  padding: 2vmax;
  border-radius: 20px;
  font-size: 4vmax;
  margin: 1rem;
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.12), 0 1px 2px rgba(0, 0, 0, 0.24);
  transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
}

.card-social:hover {
  box-shadow: 0 14px 28px rgba(0, 0, 0, 0.25), 0 3vmin 3vmin rgba(0, 0, 0, 0.22);
}

.icons a {
  text-decoration: none;
  font-size: 4vmax;
  color: #000;
  padding: 2rem;
}

@keyframes move {
  0% {
    transform: scale(1) translate(10px, -30px);
  }
  38% {
    transform: scale(0.8, 1) translate(80vw, 30vh) rotate(160deg);
  }
  40% {
    transform: scale(0.8, 1) translate(80vw, 30vh) rotate(160deg);
  }
  78% {
    transform: scale(1.3) translate(0vw, 50vh) rotate(-20deg);
  }
  80% {
    transform: scale(1.3) translate(0vw, 50vh) rotate(-20deg);
  }
  100% {
    transform: scale(1) translate(10px, -30px);
  }
}

@media screen and (max-width: 1000px) {
  .maindiv {
    flex-direction: column;
  }
  .card-social {
    padding: 10vmax;
	font-size: 5vmax;
  }
  .blob {
    width: 30vmax;
  }
  .icons a {
    padding: 2vmin;
  }
}
</style>
