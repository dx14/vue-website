<template>
<div class="wrapper">
  <i id="hand" class="far fa-hand-paper"></i>
  <h1 class="header">
    Dennis Xu
  </h1>
  <div class="body">
    Software Developer at eVestment (Nasdaq) <br>
    It's so nice to meet you!
  </div>
  <ul class="sections">
    <li>
      <router-link id="about-link" :to="{ name: 'About' }" class="link" :class="{ activelink: isActive('about') }" @mouseover.native="setActive('about')" @mouseleave.native="setInactive()">
        <i class="fas fa-user-circle icon">
          <p class="description fasdesc" :class="{ activedescription: isActive('about') }">About</p>
        </i>
      </router-link>
    </li>
    <li>
      <router-link id="work-link" :to="{ name: 'Work' }" class="link" :class="{ activelink: isActive('work') }" @mouseover.native="setActive('work')" @mouseleave.native="setInactive()">
        <i class="fas fa-briefcase icon">
          <p class="description fasdesc" :class="{ activedescription: isActive('work') }">Work</p>
        </i>
      </router-link>
    </li>
    <li>
      <a id="email-link" href="mailto:dennisxu66@gmail.com" class="link" :class="{ activelink: isActive('email') }" @mouseover="setActive('email')" @mouseleave="setInactive()">
        <i class="fas fa-envelope icon">
          <p class="description fasdesc" :class="{ activedescription: isActive('email') }">Email</p>
        </i>
      </a>
    </li>
    <li>
      <a id="github-link" href="https://github.com/dx14" target="_blank" class="link" :class="{ activelink: isActive('github') }" @mouseover="setActive('github')" @mouseleave="setInactive()">
        <i class="fab fa-github icon">
          <p class="description" :class="{ activedescription: isActive('github') }">Github</p>
        </i>
      </a>
    </li>
    <li>
      <a id="linkedin-link" href="https://www.linkedin.com/in/dennisxu6" target="_blank" class="link" :class="{ activelink: isActive('linkedin') }" @mouseover="setActive('linkedin')" @mouseleave="setInactive()">
        <i class="fab fa-linkedin icon">
          <p class="description" :class="{ activedescription: isActive('linkedin') }">LinkedIn</p>
        </i>
      </a>
    </li>
  </ul>
</div>
</template>

<script>
export default {
  name: 'Home',
  data() {
    return {
      activeItem: '',
    }
  },
  methods: {
    setActive: function(section) {
      this.activeItem = section;
    },
    setInactive: function() {
      this.activeItem = '';
    },
    isActive: function(section) {
      return this.activeItem === section;
    }
  }
}
</script>

<style scoped>

.wrapper {
  text-align: center;
  top: 50%;
  left: 50%;
  margin-left: -175px;
  margin-top: -175px;
  width: 350px;
  position: absolute;
  animation: fadeIn 2s ease;
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
}

.body {
  padding: 10px;
  font-family: 'Roboto', sans-serif;
  font-size: 15px;
  letter-spacing: 0.5px;
  color: white;
  text-shadow: 0.5px 0.5px gray;
}

.sections {
  list-style-type: none;
  padding-top: 23px;
  padding-left: 0;
  display: flex;
  justify-content: space-between;
}

.link {
  flex: 1;
  font-size: 25px;
  cursor: pointer;
  opacity: 1;
  text-shadow: 0.5px 0.5px gray;
}

.fasdesc {
  font-weight: normal;
}

.icon {
  width: 50px;
  color: white;
}

.activelink {
  opacity: 1 !important;
}

.description {
  padding-top: 8px;
  font-family: 'Roboto', sans-serif;
  font-size: 12px;
  visibility: hidden;
}

.activedescription {
  visibility: visible !important;
}

#hand {
  font-size: 50px;
  animation: rotation 1s 4 ease alternate;
  -webkit-text-stroke: 2px white;
  padding: 15px;
  color: gray;
  margin-bottom: 15px;
}

@keyframes rotation {
		from {
				-webkit-transform: rotate(0deg);
		}
		to {
				-webkit-transform: rotate(30deg);
		}
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
