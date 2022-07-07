<script setup>
import $ from "jquery"
import { onMounted } from "vue";
</script>
<script>
export default {
  mounted () {
    $(() => {
  $('.title').slideDown(4000)
  $('.name').slideDown(4000)
  $('#1').mouseover(function(){
    $('#1').css('color', 'white').css('text-shadow', '1px 1px 5px gray')
  })
    $('#1').mouseout(function(){
    $('#1').css('color', 'black').css('text-shadow', 'none')
  })
  $('#2').mouseover(function(){
    $('#2').css('color', 'white').css('text-shadow', '1px 1px 5px gray')
  })
    $('#2').mouseout(function(){
    $('#2').css('color', 'black').css('text-shadow', 'none')
  })
  $('#3').mouseover(function(){
    $('#3').css('color', 'white').css('text-shadow', '1px 1px 5px gray')
  })
    $('#3').mouseout(function(){
    $('#3').css('color', 'black').css('text-shadow', 'none')
  })
  $('#4').mouseover(function(){
    $('#4').css('color', 'white').css('text-shadow', '1px 1px 5px gray')
  })
    $('#4').mouseout(function(){
    $('#4').css('color', 'black').css('text-shadow', 'none')
  })
  $('#5').mouseover(function(){
    $('#5').css('color', 'white').css('text-shadow', '1px 1px 5px gray')
  })
    $('#5').mouseout(function(){
    $('#5').css('color', 'black').css('text-shadow', 'none')
  })
  $('#linkedin').mouseover(function(){
    $('#linkedin').css('color', 'white').css('background-color', '#0077b5').css('padding', '2px').css('border-radius', '5px')
  })
    $('#linkedin').mouseout(function(){
    $('#linkedin').css('color', 'black').css('background-color', 'white')
  })
  $('#instagram').mouseover(function(){
    $('#instagram').css('color', 'white').css('background-color', '#8A3AB9').css('padding', '2px').css('border-radius', '5px')
  })
    $('#instagram').mouseout(function(){
    $('#instagram').css('color', 'black').css('background-color', 'white')
  })
  $('#me').slideDown(4000)
})

  }
}
</script>

<template>
  <body id = 'home'>
    <div class = 'nav'>
      <p><a id = '1' href= '#aboutme'>About</a></p>
      <p><a id = '2' href= '#projects'>Projects</a></p>
      <p><a id = '3' href= '#home'>Home</a></p>
      <p><a id = '4' href= '#resume'>Resume</a></p>
      <p><a id = '5' href= '#contact'>Contact</a></p>
    </div>
  <div class = 'name'>JORDAN BANK</div>
  <div class = 'title'>Software Developer</div>
  <h1 id = 'aboutme'>hide</h1>
  <div class = 'aboutme'>
    <h1 id ='about'>About Me</h1>
    <p>I’m Jordan Bank, a software engineer and digital artist from New York City. I get excited to polish any bit of code into a meaningful product. My background as a digital artist gives me a deep appreciation  of user experience. When working on the back end, I am always visualizing the front end to ensure my vision for the final product is executed successfully.</p>
    <h4>Languages</h4>
    <p>JavaScript ES6, HTML5, CSS3, Python, TypeScript</p>
    <h4>Libraries & Frameworks</h4>
    <p>Node.js, Express.js, Django, React, Vue</p>
    <h4>Databases</h4>
    <p>MongoDB, Mongoose, ODM, SQL, PostgreSQL</p>
  </div>
  <img  id = 'me' src='https://i.imgur.com/bN4DaUR.png' alt="It's me">
  <h1 id = 'projects'>hide</h1>
  <div class = 'projects'>
    <h1 id ='project'>Projects</h1>
    <h3>This website!</h3>
    <p>This website was built from scratch using HTML5, CSS3, JavaScript, and jQuery.</p>
    <h3>The Shop</h3>
    <p>A storefront for anything you don't need - built using multiple models in React and Django. User authentication and state persistence were successfully implemented. Check it out <a id = 'shop' href="https://theshopfront.herokuapp.com/">here</a>.</p>
    <h3>PotLuck</h3>
    <p>Track the food, drinks, and supplies you're bringing to a picnic with multiple models. Built in React and Express primarily using useState and useEffect. Check it out <a id='potluck' href= 'https://agile-fortress-52444.herokuapp.com/'>here</a>.</p>
  </div>
  <h1 id = 'resume'>hide</h1>
  <div class = 'resume'>
    <h1 id = 'resumes'>Resume</h1>
    <h2>Experience</h2>
    <h3>Freelance Wedding Photographer - Jun 2018 - Nov 2021</h3>
    <p>Managed workflow for  a small team of rotating photographers and videographers at weddings and managed their payroll</p>
    <p>Used excellent communication with my  team effectively during a wedding to solve problems that arose during the event</p>
    <p>Worked on multiple post-production projects simultaneously</p>
    <h3>Freelance Graphic Designer - Jun 2018 - Feb 2022</h3>
    <p>Branded Superior Florist and the Retail Florists Alliance, both based in the northeast  </p>
    <p>Designed a NASCAR race car driven for HScott Motorsports starting in the 2013 season</p>
    <p>Delivered 100+ products to end users</p>
    <h2>Education</h2>
    <h3>General Assembly - Remote - 2022</h3>
    <p>Full-stack software engineering immersive (SEI)  student in an intensive, twelve-week, 450+ hour program focused on product development fundamentals, object-oriented programming, MVC frameworks, data modeling, and team collaboration strategies. Developed a portfolio of individual and group projects.</p>
    <h3>Stony Brook University</h3>
    <p>B.A., Political Science - 2018</p>
  </div>
  <h1 id = 'contact'>hide</h1>
  <div class = 'contact'>
    <h1 id = 'contacts'>Contact</h1>
    <p>Reach out at jordan.w.bank@gmail.com.</p>
    <p>Find me on <a id = 'linkedin' href = "https://www.linkedin.com/in/jordanwbank/">LinkedIn</a>!</p>
    <p>Check out my portrait photography work on <a id = 'instagram' href = "https://www.instagram.com/j.banksy/">Instagram</a>.</p>
  </div>
  </body>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;400&display=swap');

* {
  font-family: Roboto;
  scroll-behavior: smooth;
}

h2 {
  text-decoration: underline;
}

.nav {
  display: flex;
  justify-content: space-around;

}

button {
  background-color: grey;
  color: white;
  border-radius: 20px
}

.name {
  font-size: 60px;
  color: black;
  margin-top: 10%;
  display: none;
  text-align: center;
}

.title {
  font-size: 20px;
  color: black;
  text-align: center;
  margin: -5px;
  display: none;
}

body {
  background-image: url('https://i.imgur.com/lapBObd.jpg');
}

a {
  text-decoration: none;
  color: black;
  position: fixed;
}

#linkedin {
  text-decoration: none;
  color: black;
  position: relative;
}

#instagram {
  text-decoration: none;
  color: black;
  position: relative;
}

.aboutme {
  background-color: white;
  width:30em;
  padding: 2em;
  border-radius: 56px;
  margin-top: 20%;
  margin-left: 20%;
}


#aboutme {
  margin-top: 50%;
  color: rgba(0, 0, 0, 0);
}

#projects {
  margin-top: 50%;
  color: rgba(0, 0, 0, 0);
}

#shop {
    position: relative;
    text-decoration: underline;
}

#shop:hover {
    color: gray;
}

#potluck {
    position: relative;
    text-decoration: underline;
}

#potluck:hover {
    color: gray;
}

#resume {
  margin-top: 50%;
  color: rgba(0, 0, 0, 0);
}

#contact {
  margin-top: 50%;
  color: rgba(0, 0, 0, 0);
}

.projects {
  background-color: white;
  width: 80%;
  padding: 2em;
  border-radius: 56px;
  margin: 0 auto;
}

.resume {
  background-color: white;
  width: 80%;
  padding: 2em;
  border-radius: 56px;
  margin: 20% auto;
}

.contact {
  background-color: white;
  width: 20em;
  padding: 2em;
  border-radius: 56px;
  margin: 20% auto;
}

#me {
  display: inline-block;
  margin-left: 55%;
  margin-top: -325px;
  display: none;
}

.img {
  max-height: 245px;
  border-radius: 56px;
}

.img img:first-of-type {
  display: block;
}

@media (max-width: 900px) {
  .nav {
    display: flex;
    justify-content: flex-start;
    flex-direction: column;
  }
  a {
    text-decoration: none;
    color: black;
    position: fixed;
    font-size: 15px;
  }
  .name {
    font-size: 40px;
    color: black;
    margin-top: -20%;
    display: none;
    text-align: center;
  }
  .title {
    font-size: 15px;
    color: black;
    text-align: center;
    margin: -5px;
    display: none;
  }
  #me {
    margin: 0 14%;
    display: none;
    max-width: 350px;
  }
  .aboutme {
    background-color: white;
    max-width:300px;
    padding: 2em;
    border-radius: 56px;
    margin: 0 auto;
  }
  .projects {
    background-color: white;
    max-width: 300px;
    padding: 2em;
    border-radius: 56px;
    margin: 0 auto;
  }
  .resume {
    background-color: white;
    max-width: 300px;
    padding: 2em;
    border-radius: 56px;
    margin: 0 auto;
  }
  .carousel {
    background-color: white;
    width:14em;
    height: 150px;
    padding: 2em;
    border-radius: 56px;
    margin: 0 auto;
    align-items: center;
  }
  .img {
    max-height: 150px;
    border-radius: 56px;
  }
  .img img:first-of-type {
    display: block;
  }
  .contact {
    background-color: white;
    width: 300px;
    padding: 2em;
    border-radius: 56px;
    margin: 0 auto;
  }
}

</style>
