<template>
  <div class="main-wrapper">
    <nav class="navbar navbar-expand-lg navbar-dark bg-primary fixed-top" id="sideNav">
      <a class="navbar-brand js-scroll-trigger" href="#about">
        <span class="d-block d-lg-none">Alexandra Kromer</span>
        <span class="d-none d-lg-block">
          <img class="img-fluid img-profile rounded-circle mx-auto mb-2" src="./assets/profile.jpeg" alt="">
        </span>
      </a>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link js-scroll-trigger" href="#about">About</a>
          </li>
          <li class="nav-item">
            <a class="nav-link js-scroll-trigger" href="#experience">Experience</a>
          </li>
          <li class="nav-item">
            <a class="nav-link js-scroll-trigger" href="#education">Education</a>
          </li>
          <li class="nav-item">
            <a class="nav-link js-scroll-trigger" href="#skills">Skills</a>
          </li>
          <li class="nav-item">
            <a class="nav-link js-scroll-trigger" href="#interests">Interests</a>
          </li>
          <li class="nav-item">
            <a class="nav-link js-scroll-trigger" href="#awards">Awards</a>
          </li>
        </ul>
      </div>
    </nav>

    <div class="container-fluid p-0">

      <section class="resume-section p-3 p-lg-5 d-flex d-column" id="about">
        <div class="my-auto">
          <h1 class="mb-0">{{ name }}
            <span class="text-primary">{{ surname }}</span>
          </h1>
          <div class="subheading mb-5">{{ address }}
            <a href="mailto:alexandrakromer@gmx.de">{{ email }}</a>
          </div>
          <p class="mb-5">{{ aboutMe }}</p>
          <ul class="list-inline list-social-icons mb-0">
            <li class="list-inline-item">
              <a href="https://www.facebook.com/">
                <span class="fa-stack fa-lg">
                  <i class="fa fa-circle fa-stack-2x"></i>
                  <i class="fa fa-facebook fa-stack-1x fa-inverse"></i>
                </span>
              </a>
            </li>
            <li class="list-inline-item">
              <a href="https://twitter.com/">
                <span class="fa-stack fa-lg">
                  <i class="fa fa-circle fa-stack-2x"></i>
                  <i class="fa fa-twitter fa-stack-1x fa-inverse"></i>
                </span>
              </a>
            </li>
            <li class="list-inline-item">
              <a href="https://www.linkedin.com/in/alexandra-kromer-5a30a4170/">
                <span class="fa-stack fa-lg">
                  <i class="fa fa-circle fa-stack-2x"></i>
                  <i class="fa fa-linkedin fa-stack-1x fa-inverse"></i>
                </span>
              </a>
            </li>
            <li class="list-inline-item">
              <a href="https://github.com/">
                <span class="fa-stack fa-lg">
                  <i class="fa fa-circle fa-stack-2x"></i>
                  <i class="fa fa-github fa-stack-1x fa-inverse"></i>
                </span>
              </a>
            </li>
          </ul>
        </div>
      </section>

      <section class="resume-section p-3 p-lg-5 d-flex flex-column" id="experience">
        <div class="my-auto">
          <h2 class="mb-5">Experience</h2>

          <div class="resume-item d-flex flex-column flex-md-row mb-5" v-for="job in experience" :key="job.description">
            <div class="resume-content mr-auto">
              <h3 class="mb-0">{{ job.position }}</h3>
              <div class="subheading mb-3">{{ job.company }}</div>
              <p>{{ job.description }}</p>
            </div>
            <div class="resume-date text-md-right">
              <span class="text-primary">{{ job.startDate }} - {{ job.endDate }}</span>
            </div>
          </div>

        </div>

      </section>

      <section class="resume-section p-3 p-lg-5 d-flex flex-column" id="education">
        <div class="my-auto">
          <h2 class="mb-5">Education</h2>

          <div class="resume-item d-flex flex-column flex-md-row mb-5">
            <div class="resume-content mr-auto">
              <h3 class="mb-0">Albert-Ludwigs University in Freiburg im Breisgau, Germany</h3>
              <div class="subheading mb-3">Master of Science in Business Administration</div>
            </div>
            <div class="resume-date text-md-right">
              <span class="text-primary">October 2017 - Present</span>
            </div>
          </div>

           <div class="resume-item d-flex flex-column flex-md-row">
            <div class="resume-content mr-auto">
              <h3 class="mb-0">Hanken School of Economics in Helsinki, Finland</h3>
              <div class="subheading mb-3">International Helsinki Days (seminar)</div>
              <p> </p>
            </div>
            <div class="resume-date text-md-right">
              <span class="text-primary">February 2019</span>
            </div>
          </div>

          <div class="resume-item d-flex flex-column flex-md-row">
            <div class="resume-content mr-auto">
              <h3 class="mb-0">Alma Mater Studiorum Universita di Bologna in Bologna, Italy</h3>
              <div class="subheading mb-3">ERASMUS student exchange</div>
              <p> </p>
            </div>
            <div class="resume-date text-md-right">
              <span class="text-primary">September 2018 - January 2019</span>
            </div>
          </div>

          <div class="resume-item d-flex flex-column flex-md-row">
            <div class="resume-content mr-auto">
              <h3 class="mb-0">Albert-Ludwigs University in Freiburg im Breisgau, Germany</h3>
              <div class="subheading mb-3">Bachelor of Science in Economics</div>
              <p>Final Grade: 1.3 with distinction very good </p>
            </div>
            <div class="resume-date text-md-right">
              <span class="text-primary">October 2014 - August 2017</span>
            </div>
          </div>

          <div class="resume-item d-flex flex-column flex-md-row">
            <div class="resume-content mr-auto">
              <h3 class="mb-0">Wentzinger Gymnasium in Freiburg im Breisgau, Germany</h3>
              <div class="subheading mb-3">High School</div>
              <p>Final Grade: 2.4 with distinction "good"</p>
            </div>
            <div class="resume-date text-md-right">
              <span class="text-primary">September 2012 - July 2014</span>
            </div>
          </div>

        </div>
      </section>

      <section class="resume-section p-3 p-lg-5 d-flex flex-column" id="skills">
        <div class="my-auto">
          <h2 class="mb-5">Skills</h2>

          <div class="subheading mb-3">Languages</div>
          <ul class="fa-ul mb-0">
            <li>
              <i class="fa-li fa fa-check"></i> German (native language) </li>
            <li>
              <i class="fa-li fa fa-check"></i> English (C1)</li>
            <li>
              <i class="fa-li fa fa-check"></i> Latin (Latinum)</li>
            <li>
              <i class="fa-li fa fa-check"></i> French (A2)</li>

          </ul>
          <br>

          <div class="subheading mb-3">Computer Skills &amp; Tools</div>
          <ul class="fa-ul mb-0">
            <li>
              <i class="fa-li fa fa-check"></i>
              Microsoft Windows</li>
            <li>
              <i class="fa-li fa fa-check"></i>
              MS Office</li>
            <li>
              <i class="fa-li fa fa-check"></i>
              Mac OS</li>
            <li>
              <i class="fa-li fa fa-check"></i>
              SQL</li>
            <li>
              <i class="fa-li fa fa-check"></i>
              R Studio</li>
            <li>
               <i class="fa-li fa fa-check"></i>
              SPSS</li>
            <li>
              <i class="fa-li fa fa-check"></i>
              IBM Watson</li>
          </ul>

        </div>
      </section>

      <section class="resume-section p-3 p-lg-5 d-flex flex-column" id="interests">
        <div class="my-auto">
          <h2 class="mb-5">Interests</h2>
          <p>Apart from being a Master student and expanding my skillset with eLearning courses, I enjoy most of my time being physically active in the nature with running and biking as well as hiking in beautiful landscapes. Throughout the year I follow various workouts in addition to inline skating. </p>
          <p class="mb-0">When forced indoors, I enjoy a good book and I follow a number of podcasts on critical thinking or self improvement strategies. I am an aspiring chef, and I spend a large amount of my free time trying out new recipes.</p>
        </div>
      </section>
      <section class="resume-section p-3 p-lg-5 d-flex flex-column" id="awards">
        <div class="my-auto">
          <h2 class="mb-5">Awards &amp; Certifications</h2>
          <ul class="fa-ul mb-0">
            <li>
              <i class="fa-li fa fa-trophy text-warning"></i>
              <p>To be updated</p>
            </li>

          </ul>
        </div>
      </section>

    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      title: 'My portfolio',
      name: 'Alexandra',
      surname: 'Kromer',
      address: '+49 (0) 151 419 00 616 ·',
      email: 'alexandrakromer@gmx.de',
      aboutMe: 'I am a Master student in Business Administration at the Albert-Ludwigs University in Freiburg im Breisgau.',
      experience: [
        {
          position: 'Erasmus Assistant',
          company: 'Albert-Ludwigs University Freiburg, Germany',
          description: 'Support and nomination for Incoming and Outgoing exchange students, supervision and maintenance of the International Programs Office website of the department of economics, support for partner universities',
          startDate: 'October 2016',
          endDate: 'Present'
        },
        {
          position: 'Tutor for Mathematics and Microeconomics',
          company: 'Albert-Ludwigs University Freiburg, Germany',
          description: 'Preparing and leading teaching supportive exercises for students, independent preparation and execution of exam preparation courses, supervision and correction of exams, mentoring',
          startDate: 'November 2015',
          endDate: 'Present'
        },
        {
          position: 'Marketing Intern',
          company: 'Chilcotin Holidays in Gold Bridge, Canada',
          description: 'Creating and communicating packages for client trips in the Chilcotin Mountains',
          startDate: 'August 2015',
          endDate: 'September 2015'
        }
      ]
    }
  },
  mounted () {
    const $ = this.jquery
    this.$nextTick(() => {
      // our custom jQuery code goes here
      $('a.js-scroll-trigger[href*="#"]:not([href="#"])').click(function () {
        if (location.pathname.replace(/^\//, '') === this.pathname.replace(/^\//, '') && location.hostname === this.hostname) {
          var target = $(this.hash)
          target = target.length ? target : $('[name=' + this.hash.slice(1) + ']')
          if (target.length) {
            $('html, body').animate({
              scrollTop: (target.offset().top)
            }, 1000, 'easeInOutExpo')
            return false
          }
        }
      })

      // Closes responsive menu when a scroll trigger link is clicked
      $('.js-scroll-trigger').click(function () {
        $('.navbar-collapse').collapse('hide')
      })

      // Activate scrollspy to add active class to navbar items on scroll
      $('body').scrollspy({
        target: '#sideNav'
      })
    })
  }
}
</script>

<style>

</style>
