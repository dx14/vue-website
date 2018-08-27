<template>
  <div class="wrapper">
    <h1 class="header">
      Work & Skills
    </h1>
    <div class="body">
      <h3 class="subheader">Work</h3>
      <p>
      <ul class="work-section">
        <li>
          <p class="work-item">eVestment (Nasdaq)</p>
          <ul>
            <li>
              Full-Stack Software Developer
            </li>
            <li>
              Software Developer Intern
            </li>
          </ul>
          <p class="work-item">Duke University</p>
          <ul>
            <li>
              Data Structures and Algorithms UTA
            </li>
          </ul>
          <p class="work-item">DukeEngage: Zhuhai, China</p>
          <ul>
            <li>
              Student Instructor
            </li>
          </ul>
        </li>
      </ul>
      <br>
      </p>
      <h3 class="subheader">Skills</h3>
      <p>
        Java | C# | .NET | Python | Javascript | Vue | Swift | SQL | AWS | Git
      </p>
    </div>
  </div>
  </div>
</template>

<script>
export default {
    name: 'Work'
}
</script>

<style scoped>

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

.body {
  padding: 10px;
  font-family: 'Roboto', sans-serif;
  font-size: 15px;
  letter-spacing: 0.5px;
  color: white;
  text-shadow: 0.5px 0.5px gray;
  text-align: justify;
}

.work-section {
  list-style: none;
}

.work {
  margin: 0;
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
