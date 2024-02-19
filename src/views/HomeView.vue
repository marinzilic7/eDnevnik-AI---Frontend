<script setup>
import Navbar from "@/components/Navbar.vue";
import Footer from "@/components/Footer.vue";
</script>

<template>
  <Navbar />
  <div class="container">
    <div
      class="items d-flex flex-column align-items-center justify-content-center mt-5"
    >
      <h1 class="fw-bold mt-5 heading">
        AI Pomoćnik za <span style="color: #056069">eDnevnik</span>
      </h1>
      <p class="fs-4 descHeading" style="color: #616161">
        Ovaj sustav Vam pomaže u radu sa eDnevnik aplikacijom.
      </p>
      <div class="mb-4 mt-4 col-12 col-lg-9 col-xl-9 col-md-12 col-sm-12 position-relative">
        <input
          class="form-control searchBar"
          type="text"
          placeholder="Postavite pitanje..."
          aria-label="Search"
        />
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="25"
          height="25"
          fill="#056069"
          class="bi bi-search position-absolute"
          viewBox="0 0 16 16"
          style="right: 20px; top: 50%; transform: translateY(-50%)"
        >
          <path
            d="M11.742 10.344a6.5 6.5 0 1 0-1.397 1.398h-.001q.044.06.098.115l3.85 3.85a1 1 0 0 0 1.415-1.414l-3.85-3.85a1 1 0 0 0-.115-.1zM12 6.5a5.5 5.5 0 1 1-11 0 5.5 5.5 0 0 1 11 0"
          />
        </svg>
      </div>
      <div class="questionItems mt-4 d-flex  justify-content-between col-12 col-lg-6 col-xl-6 col-md-10 col-sm-12">
        <p>Kako unijeti ocjenu?</p>
        <p>Gdje se nalazi raspored sati?</p>
        <p>Ne radi prijava?</p>
      </div>
      <div class="col-12 col-md-5 col-sm-5 col-lg-3 col-xl-3 mt-3">
        <button class="btn text-light p-3 w-100 fs-4 mt-4 bgBtn">Pošalji upit</button>
      </div>
      <p class="mt-2" style="color: #616161;">Imate poteškoća, javite nam se.</p>
      <br>
      <br>
      <div class="mt-5 bottomImages">
        <img src="../assets/images/tehnicka.png" height="100px" width="300px" alt="">
        <img src="../assets/images/sumAi.png"  height="50px" width="150px" alt="">
      </div>
    </div>
  </div>
    <Footer />
</template>

<style scoped>

.heading{
    font-size: 50px;
}
.searchBar {
  border-radius: 50px;
  padding: 15px;
  box-shadow: none;
}

.searchBar::placeholder{
    color:#959595;
}

.searchBar:focus {
  box-shadow: none;
  border: 1px solid #056069;
}
.questionItems p {
  background-color: #fff;
  padding: 15px;
  border-radius: 50px;
  color: #056069;
}

.bgBtn{
    background-color: #056069;
    border-radius: 50px;
}

@media only screen and (max-width: 576px){
    .heading{
        font-size: 30px;
        margin:0 !important;
    }

    .descHeading{
        font-size: 15px !important;
    }

   .questionItems{
    display: flex;
    flex-direction: column;
    text-align: center;
    margin: 0 !important;
   }

   .bgBtn{
        font-size: 16px !important;
        margin:0 !important;
   }

   .bottomImages{
    display: flex;
    margin:10px !important;
   }
   .bottomImages img{
        width:150px;
        height: 50px;
   }

   
}
</style>
