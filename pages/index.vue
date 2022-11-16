<template>
  <div>
    <div class="absolute top-0 left-0 w-screen" style="z-index: -10; background-image: url('/bg.svg'); background-size: cover; background-position: bottom; height: 700px;">
    </div>
    <div class="flex flex-col lg:flex-row mt-16 lg:mt-0 justify-center lg:justify-start">
      <div class="flex-1 flex flex-col items-center lg:items-end justify-center lg:mr-16">
        <div>
          <h1 class="text-5xl font-bold text-red-400">
            Miejsce gdzie <br/>
            kreatywność spotyka<br/>
            się z
            <span class="underline underline-offset-2">technologią</span>
          </h1>
          <div class="flex flex-row items-center">
            <button class="mt-6 px-7 py-1 rounded-xl border-2 border-solid border-red-400 font-semibold text-red-400 hover:bg-red-400 hover:border-transparent hover:text-white duration-100">
              więcej
            </button>
            <button class="mt-6 ml-2 px-4 py-1 flex justify-end items-center text-gray-500">
              moje projekty <i class='bx bx-right-arrow-alt'></i>
            </button>
          </div>
          
        </div>
      </div>


      <div class="flex-1">
        <div class="relative w-96 mt-16 left-16">
          <img src="/jessi.png" placeholder loading='lazy' alt="gamedevlady" class="ladyImage"/>
          <img src="/game development.png" placeholder loading='lazy' alt="game development" class="spinAnimation absolute -right-10 -top-8"/>
        </div>
      </div>
      
    </div>
    <div class="container mx-auto">

      <div class="my-24 lg:mt-48 text-center">
        <h2 class="textPrim text-2xl font-semibold mb-4">Sprawdź co sam możesz stworzyć</h2>
        <p class="px-16 textSec mb-6">
          Zobacz co samemu możesz zrobić dzięki moim poradnikom do jednego z czołowych silników gier
        </p>
        <button class="px-8 py-2 bg-red-400 rounded-xl text-white hover:bg-red-300 duration-100">
          Moje materiały
        </button>
      </div>

      <div class="bubble relative my-24 py-16 bg-red-400 px-12 xl:px-80 text-center md:text-left text-white rounded-3xl">
        <div class="max-w-2xl">
          <h2 class="text-2xl mb-8 md:ml-16">Lorem ipsum</h2>
          <p class="text-left mb-6">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Levatio igitur vitiorum magna fit in iis, qui habent ad virtutem progressionis aliquantum. Quacumque enim ingredimur, in aliqua historia vestigium ponimus. Respondent extrema primis, media utrisque, omnia omnibus. Quod cum dixissent, ille contra. Similiter sensus, cum accessit ad naturam, tuetur illam quidem, sed etiam se tuetur; Duo Reges: constructio interrete. Nullus est igitur cuiusquam dies natalis.
          </p>
          <div class="w-full text-left mb-8">
            <button class="px-8 py-2 bg-white rounded-xl text-red-400 hover:bg-gray-200 duration-100">
              Moje materiały
            </button>
          </div>
        </div>
        
        <div class="flex text-white space-x-6 mb-6 lg:justify-end">
          <div class="text-left">

            <div class="text-6xl font-semibold">
              7+
            </div>
            <div>
              lat doświadczenia
            </div>
 
          </div>
          <div class="text-left">

            <div class="text-6xl font-semibold">
                2
            </div>
            <div>
                projekty komercyjne
            </div>

          </div>
        </div>
      </div>

      <div class="my-24 text-center">
        <h2 class="textPrim text-2xl mb-2 font-semibold">
          Moje projekty
        </h2>

        <div class="px-8 lg:flex lg:justify-center lg:space-x-8">
          <div class="my-12 text-center flex flex-col items-center">
            <a href="https://store.steampowered.com/app/842180/Prison_Simulator/" target="_blank">
              <nuxt-img src="ps.jpg" alt="Game Prison Simulator logo" sizes="250px lg:500px" class="mb-3" />
              <p class="textSec">Prison Simulator</p>
            </a>
          </div>
          <div class="my-12 text-center flex flex-col items-center">
            <a href="https://store.steampowered.com/app/1561660/The_Lightbringer/" target="_blank">
              <nuxt-img src="tl.jpg" alt="game The Lightbringer logo" sizes="250px lg:500px" class="mb-3" />
              <p class="textSec">The Lightbringer</p>
            </a>
          </div>
        </div>
      </div>

    </div>

  
  </div>
</template>

<script>
export default {
  name: 'IndexPage'
}
</script>

<style>
  body{
    font-family: 'Roboto', sans-serif;
  }

  .spinAnimation{
    animation-name: spin;
    animation-duration: 5000ms;
    animation-iteration-count: infinite;
    animation-timing-function: linear;
  }

  @keyframes spin {
    from {
        transform:rotate(0deg);
    }
    to {
        transform:rotate(-360deg);
    }
  }
</style>