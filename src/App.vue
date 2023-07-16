<script setup>
const landingPage="Start Landing Page"
const SignupButton="Sign Up"

const title="Generate more leads with a professional landing page!"
const submitButton="Submit"

const windowIcon="bi-window m-auto text-primary"
const responsive="Fully Responsive"
const responsivePara="This theme will look great on any device, no matter the size!"
const layerIcon="bi-layers m-auto text-primary"
const bootstrap="Bootstrap 5 Ready"
const bootstrapPara="Featuring the latest build of the new Bootstrap 5 framework!"
const terminalIcon="bi-terminal m-auto text-primary"
const easy="Easy to Use"
const easyPara="Ready to use with your own content, or customize the source files!"

const responsiveImg="background-image: url('src/assets/img/bg-showcase-1.jpg')"
const responsiveHeading="Fully Responsive Design"
const responsiveDetail="When you use a theme created by Start Bootstrap, you know that the theme will look great on any device, whether it's a phone, tablet, or desktop the page will behave responsively!"
const bootstrapImg="background-image: url('src/assets/img/bg-showcase-2.jpg')"
const bootstrapHeading="Updated For Bootstrap 5"
const bootstrapDetail="Newly improved, and full of great utility classes, Bootstrap 5 is leading the way in mobile responsive web development! All of the themes on Start Bootstrap are now using Bootstrap 5!"
const easyImg="background-image: url('src/assets/img/bg-showcase-3.jpg')"
const easyHeading="Easy to Use & Customize"
const easyDetail="Landing Page is just HTML and CSS with a splash of SCSS for users who demand some deeper customization options. Out of the box, just add your content and images, and your new landing page will be ready to go!"

const testimonialHeading="What people are saying..."
const testimonialImg1="src/assets/img/testimonials-1.jpg"
const testimonialName1="Margaret E."
const testimonialComment1="This is fantastic! Thanks so much guys!"
const testimonialImg2="src/assets/img/testimonials-2.jpg"
const testimonialName2="Fred S."
const testimonialComment2="Bootstrap is amazing. I've been using it to create lots of super nice landing pages."
const testimonialImg3="src/assets/img/testimonials-3.jpg"
const testimonialName3="Sarah W."
const testimonialComment3="Thanks so much for making these free resources available to us!"

const actionHeading="Ready to get started? Sign up now!"

const about="About"
const contact="Contact"
const terms="Terms of Use"
const privacy="Privacy Policy"
const footerPara="Your Website 2023. All Rights Reserved."
const fbIcon="bi-facebook fs-3"
const twIcon="bi-twitter fs-3"
const instaIcon="bi-instagram fs-3"

</script>

<template>
  <!-- Navigation-->
  <nav class="navbar navbar-light bg-light static-top">
    <div class="container">
      <a class="navbar-brand" href="#!">{{landingPage}}</a>
      <a class="btn btn-primary" href="#signup">{{SignupButton}}</a>
    </div>
  </nav>

  <!-- Masthead-->
  <header class="masthead">
    <div class="container position-relative">
      <div class="row justify-content-center">
        <div class="col-xl-6">
          <div class="text-center text-white">
            <!-- Page heading-->
            <h1 class="mb-5">{{title}}</h1>
              <!-- Email address input-->
              <div class="row">
                <div class="col">
                  <input class="form-control form-control-lg" id="emailAddress" type="email" placeholder="Email Address" data-sb-validations="required,email" />
                </div>
                <div class="col-auto"><button class="btn btn-primary btn-lg disabled" id="submitButton" type="submit">{{submitButton}}</button></div>
              </div>
          </div>
        </div>
      </div>
    </div>
  </header>

  <!-- Icons Grid-->
  <section class="features-icons bg-light text-center">
    <div class="container">
      <div class="row">
        <div class="col-lg-4">
          <div class="features-icons-item mx-auto mb-5 mb-lg-0 mb-lg-3">
            <div class="features-icons-icon d-flex"><i :class="windowIcon"></i></div>
            <h3>{{responsive}}</h3>
            <p class="lead mb-0">{{responsivePara}}</p>
          </div>
        </div>
        <div class="col-lg-4">
          <div class="features-icons-item mx-auto mb-5 mb-lg-0 mb-lg-3">
            <div class="features-icons-icon d-flex"><i :class="layerIcon"></i></div>
            <h3>{{bootstrap}}</h3>
            <p class="lead mb-0">{{bootstrapPara}}</p>
          </div>
        </div>
        <div class="col-lg-4">
          <div class="features-icons-item mx-auto mb-0 mb-lg-3">
            <div class="features-icons-icon d-flex"><i :class="terminalIcon"></i></div>
            <h3>{{easy}}</h3>
            <p class="lead mb-0">{{easyPara}}</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Image Showcases-->
  <section class="showcase">
    <div class="container-fluid p-0">
      <div class="row g-0">
        <div class="col-lg-6 order-lg-2 text-white showcase-img" :style="responsiveImg"></div>
        <div class="col-lg-6 order-lg-1 my-auto showcase-text">
          <h2>{{responsiveHeading}}</h2>
          <p class="lead mb-0">{{responsiveDetail}}</p>
        </div>
      </div>
      <div class="row g-0">
        <div class="col-lg-6 text-white showcase-img" :style="bootstrapImg"></div>
        <div class="col-lg-6 my-auto showcase-text">
          <h2>{{bootstrapHeading}}</h2>
          <p class="lead mb-0">{{bootstrapDetail}}</p>
        </div>
      </div>
      <div class="row g-0">
        <div class="col-lg-6 order-lg-2 text-white showcase-img" :style="easyImg"></div>
        <div class="col-lg-6 order-lg-1 my-auto showcase-text">
          <h2>{{easyHeading}}</h2>
          <p class="lead mb-0">{{easyDetail}}</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Testimonials-->
  <section class="testimonials text-center bg-light">
    <div class="container">
      <h2 class="mb-5">{{testimonialHeading}}</h2>
      <div class="row">
        <div class="col-lg-4">
          <div class="testimonial-item mx-auto mb-5 mb-lg-0">
            <img class="img-fluid rounded-circle mb-3" :src="testimonialImg1" alt="..." />
            <h5>{{testimonialName1}}</h5>
            <p class="font-weight-light mb-0">"{{testimonialComment1}}"</p>
          </div>
        </div>
        <div class="col-lg-4">
          <div class="testimonial-item mx-auto mb-5 mb-lg-0">
            <img class="img-fluid rounded-circle mb-3" :src="testimonialImg2" alt="..." />
            <h5>{{testimonialName2}}</h5>
            <p class="font-weight-light mb-0">"{{testimonialComment2}}"</p>
          </div>
        </div>
        <div class="col-lg-4">
          <div class="testimonial-item mx-auto mb-5 mb-lg-0">
            <img class="img-fluid rounded-circle mb-3" :src="testimonialImg3" alt="..." />
            <h5>{{testimonialName3}}</h5>
            <p class="font-weight-light mb-0">"{{testimonialComment3}}"</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Call to Action-->
  <section class="call-to-action text-white text-center" id="signup">
    <div class="container position-relative">
      <div class="row justify-content-center">
        <div class="col-xl-6">
          <h2 class="mb-4">{{actionHeading}}</h2>
          <!-- Email address input-->
            <div class="row">
              <div class="col">
                <input class="form-control form-control-lg" id="emailAddressBelow" type="email" placeholder="Email Address" data-sb-validations="required,email" />
              </div>
              <div class="col-auto"><button class="btn btn-primary btn-lg disabled" id="submitButton" type="submit">{{submitButton}}</button></div>
            </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Footer-->
  <footer class="footer bg-light">
    <div class="container">
      <div class="row">
        <div class="col-lg-6 h-100 text-center text-lg-start my-auto">
          <ul class="list-inline mb-2">
            <li class="list-inline-item"><a href="#!">{{about}}</a></li>
            <li class="list-inline-item">⋅</li>
            <li class="list-inline-item"><a href="#!">{{contact}}</a></li>
            <li class="list-inline-item">⋅</li>
            <li class="list-inline-item"><a href="#!">{{terms}}</a></li>
            <li class="list-inline-item">⋅</li>
            <li class="list-inline-item"><a href="#!">{{privacy}}</a></li>
          </ul>
          <p class="text-muted small mb-4 mb-lg-0">&copy;{{footerPara}}</p>
        </div>
        <div class="col-lg-6 h-100 text-center text-lg-end my-auto">
          <ul class="list-inline mb-0">
            <li class="list-inline-item me-4">
              <a href="#!"><i :class="fbIcon"></i></a>
            </li>
            <li class="list-inline-item me-4">
              <a href="#!"><i :class="twIcon"></i></a>
            </li>
            <li class="list-inline-item">
              <a href="#!"><i :class="instaIcon"></i></a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </footer>
</template>

<style scoped>

</style>
