<template>
  <div class="wrapper">
    <h1 class="header">
      About
    </h1>
    <div class="row">
    <div class="bodycolumn body">
      <p>
      Hello there! My name is Dennis Xu. I grew up in Columbus, GA, graduated from Duke University in 2017, and
      am currently working as a full-stack software developer at eVestment (Nasdaq) in Atlanta, GA.
      I first discovered computer science in college, and ever since then I've been amazed at the creativity,
      innovation, and collaboration that goes into creating software. <br> <br>

      I'm especially passionate about front-end web and iOS development because I love
      watching an app grow visually as I build it. Besides coding, I also enjoy photography,
      teaching, and conversation. <br><br>
      </p>
    </div>
    <div class="photocolumn">
      <img class="photo" src="../assets/aboutme.jpg">
    </div>
  </div>
  </div>
</template>

<script>
export default {
    name: 'About'
}
</script>

<style scoped>
.body {

}

.wrapper {
  text-align: center;
  top: 50%;
  left: 50%;
  margin-left: -300px;
  margin-top: -200px;
  width: 600px;
  position: absolute;
  animation: fadeIn 1s ease;
}

.header {
  font-size: 50px;
  color: white;
  text-align: center;
  font-family: 'Roboto', sans-serif;
  font-weight: bolder;
  font-size: 50px;
  text-shadow: 1px 1px gray;
  text-transform: uppercase;
  letter-spacing: 5px;
  padding-bottom: 20px;
}

.row {
  display: flex;
}

.body {
  padding: 10px;
  font-family: 'Roboto', sans-serif;
  font-size: 15px;
  letter-spacing: 0.5px;
  color: white;
  text-shadow: 0.5px 0.5px gray;
}

.bodycolumn {
  flex: 60%;
  text-align: justify;
}

.photocolumn {
  flex: 40%;
  padding-top: 5px;
}

.photo {
  width: 90%;
  height: auto;
  border-radius: 20px;
  border: 5px solid #f45f42;
}

@keyframes fadeIn {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}
</style>
