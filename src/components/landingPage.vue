<template>
  <div>
    <!-- #region navbar -->
    <nav class="navbar fixed-top navbar-expand-lg navbar-dark bg-dark">
      <a class="navbar-brand" href="#">Jeff Smith</a>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false"
        aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link" href="#">About Me
              <span class="sr-only">(current)</span>
            </a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Resume</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Portfolio</a>
          </li>
        </ul>
      </div>
    </nav>
    <!-- #endregion navbar -->
    <div class="jumbotron">
      <!-- #region cards -->
      <div>
        <h1>Resume</h1>
      </div>
      <div class="card-deck row">
        <div class="card">
          <img class="card-img-top" src="http://via.placeholder.com/290x150" alt="Card image cap">
          <div class="card-body">
            <h5 class="card-title">Experience</h5>
            <p class="card-text">This is a longer card with supporting text below as a natural lead-in to additional content. This content is
              a little bit longer.</p>
            <p class="card-text">
              <small class="text-muted">Last updated 3 mins ago</small>
            </p>
          </div>
        </div>
        <div class="card flip-container" ontouchstart="this.classList.toggle('hover');">
          <img class="card-img-top center imgthumbnail" src="../assets/images/cap.png" alt="Card image cap">
          <div class="card-body">

            <div class="flipper">
              <div class="front">
                <!-- front content -->
                <h1 class="card-title">Education</h1>
                <div class="card-text">
                    <blockquote class="blockquote mb-0">
                        <p>Education is the foundation upon which we build our future.</p>
                        <footer class="blockquote-footer">Christine Gregoire</footer>
                      </blockquote>
                  </div>
              </div>
              <div class="back">
                <!-- back content -->
                <p>
                  <strong> Code Works, Boise, ID</strong> Full-Stack Web Development – JavaScript, C#, SQL, vue.js, node.js, HTML
                  and CSS
                </p>
                <p>
                  <strong>Utah State University, Logan, UT</strong> Bachelor of Arts – Accounting, Minor in Economics and Spanish
                </p>
              </div>
            </div>

          </div>
        </div>
        <div class="card">
          <img class="card-img-top" src="http://via.placeholder.com/290x150" alt="Card image cap">
          <div class="card-body">
            <h5 class="card-title">Skills</h5>
            <p class="card-text">This is a wider card with supporting text below as a natural lead-in to additional content. This card has even
              longer content than the first to show that equal height action.</p>
            <p class="card-text">
              <small class="text-muted">Last updated 3 mins ago</small>
            </p>
          </div>
        </div>
      </div>
      <!-- #endregion cards -->
      <!-- #region carousel -->
<div>
  <h1>Portfolio</h1>
</div>
      <div class="row">
        <div id="carouselExampleIndicators" class="carousel slide col-md-6 offset-md-3" data-ride="carousel">
          <ol class="carousel-indicators">
            <li data-target="#carouselExampleIndicators" data-slide-to="0" class="active"></li>
            <li data-target="#carouselExampleIndicators" data-slide-to="1"></li>
            <li data-target="#carouselExampleIndicators" data-slide-to="2"></li>
            <li data-target="#carouselExampleIndicators" data-slide-to="3"></li>
          </ol>
          <div class="carousel-inner border">
            <div class="carousel-item active">
              <img class="d-block w-100" src="http://via.placeholder.com/290x150" alt="First slide">
              <div class="carousel-caption d-none d-md-block">
                <h5>Test Title 1</h5>
                <p>woot</p>
              </div>
            </div>
            <div class="carousel-item">
              <img class="d-block w-100" src="http://via.placeholder.com/290x150" alt="Second slide">
              <div class="carousel-caption d-none d-md-block">
                <h5>Test Title 2</h5>
                <p>wootier</p>
              </div>
            </div>
            <div class="carousel-item">
              <img class="d-block w-100" src="http://via.placeholder.com/290x150" alt="Third slide">
              <div class="carousel-caption d-none d-md-block">
                <h5>Test Title 3</h5>
                <p>wootiest</p>
              </div>
            </div>
            <div class="carousel-item">
              <img class="d-block w-100" src="http://via.placeholder.com/290x150" alt="Third slide">
              <div class="carousel-caption d-none d-md-block">
                <h5>Test Title 4</h5>
                <p>wootiested</p>
              </div>
            </div>
          </div>
          <a class="carousel-control-prev" href="#carouselExampleIndicators" role="button" data-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="sr-only">Previous</span>
          </a>
          <a class="carousel-control-next" href="#carouselExampleIndicators" role="button" data-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="sr-only">Next</span>
          </a>
        </div>
      </div>
      <!-- #endregion carousel -->
      <!-- #region Social -->
      <div>

      </div>
      <!-- #endregion Social -->
    </div>
  </div>
</template>


<script>
  export default {
    name: '',
    data() {
      return {}
    },
    computed: {},
    methods: {},
    components: {}
  }
</script>


<style scoped>
  .card-deck {
    margin-bottom: 4rem;
    margin-top: 2em;
  }

  .center {

    display: block;
    margin-left: auto;
    margin-right: auto;
    width: 50%;

  }

  .imgthumbnail {
    width: 65%;
    /* you can use % */
    height: auto;
  }

  .jumbotron {
    background-color: rgba(124, 124, 124, 0);
  }



  /* entire container, keeps perspective */

  .flip-container {
    perspective: 1000;
  }

  /* flip the pane when hovered */

  .flip-container:hover .flipper,
  .flip-container.hover .flipper {
    transform: rotateY(180deg);
  }



  /* flip speed goes here */

  .flipper {
    transition: .8s;
    transform-style: preserve-3d;

    position: relative;
  }

  /* hide back of pane during swap */

  .front,
  .back {
    backface-visibility: hidden;

    position: absolute;
    top: 0;
    left: 0;
  }

  /* front pane, placed above back */

  .front {
    z-index: 2;
    /* for firefox 31 */
    transform: rotateY(0deg);
  }

  /* back, initially hidden pane */

  .back {
    transform: rotateY(180deg);

  }
</style>