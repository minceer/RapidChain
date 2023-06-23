<template>
  <div class="w-full min-h-screen aspect-auto bg-no-repeat bg-contain" style="background-image: url(/bg.png);">
    <div class="w-full h-max  top-0 z-50 bg- fixed backdrop-blur-md py-4 lg:py-8">
      <div class="flex w-full container justify-between  mx-auto 2xl:px-0">
        <div class="flex gap-4 items-center h-max my-auto w-max">

          <h1 class="text-3xl pl-8 lg:pl-0 w-max uppercase text-regular text-neutral-800">Rapid Chain</h1>
        </div>
        <button class="mx-4 hidden" @click="aside=!aside" >
          <Icon icon="ic:round-menu" class="text-3xl text-neutral-900" />
        </button>
        <div :class="aside ? 'flex' : 'hidden'">
          <div class="fixed inset-0 bg-black bg-opacity-50 z-50" :class="aside ? 'flex' : 'hidden'"
            @click="aside = false"></div>
          <div class="fixed inset-y-0 right-0 w-64 bg-white z-50" :class="aside ? 'flex' : 'hidden'">
            <div class="flex flex-col gap-4 p-4">
              <button class="mx-4" @click="aside = false">
                <Icon icon="ic:round-close" class="text-3xl text-neutral-900" />
              </button>
              <a class="text-xl hover:text-green-600 text-gray-600 text-regular" href="#home">Home</a>
              <a class="text-xl hover:text-green-600 text-gray-600 text-regular" href="#adventage">Adventage</a>
              <a class="text-xl hover:text-green-600 text-gray-600 text-regular" href="#roadMap">Roadmap</a>
            </div>
          </div>
        </div>
        <div class="hidden md:flex gap-10 h-max my-auto">
          <a class="text-xl hover:text-green-600 text-gray-600 text-regular" href="#home">Home</a>
          <a class="text-xl hover:text-green-600 text-gray-600 text-regular" href="#adventage">Adventage</a>
          <a class="text-xl hover:text-green-600 text-gray-600 text-regular" href="#roadMap">Roadmap</a>
        </div>
      </div>
    </div>
    <section id="home" class="container mx-auto bg-fixed 2xl:px-0 pt-20 px-4 lg:px-0">
      <div class="w-full flex flex-col-reverse md:flex-row gap-2">
        <div class="flex flex-col relative w-full z-20">
          <p class="text-neutral-900 text-4xl md:text-[110px] md:leading-[106px] text-bold mt-20">The first modular <br
              class="md:block hidden"> blockchain <br class="md:block hidden"> network</p>
          <p class="mt-4 text-neutral-900/80 md:mt-16 text-regular text-normal md:text-xl">Rapid Chain is a modular
            consensus and data network, built to enable <br class="md:block hidden"> anyone to
            easily deploy their own blockchain with minimal overhead.</p>
        </div>
        <img class="aspect-square md:my-auto max-w-xs mt-10 md:max-w-lg lg:right-48 lg:absolute mx-auto md:mt-20"
          src="./assets/logo.png" alt="Vue logo" />
      </div>
    </section>
    <section id="adventage" class="container mx-auto bg-fixed mt-20 px-4 lg:px-0">
      <h1 class="lg:text-7xl text-4xl text-neutral-900 text-bold text-left">Adventage</h1>
      <div class="grid grid-cols-4 gap-2 mt-10">
        <div
          class="col-span-4 md:col-span-1 py-[35px] px-[25px] flex flex-col backdrop-blur-md shadow-lg w-full rounded-md transition-all hover:shadow-2xl">
          <img src="./assets/advantage-1.png" class="aspect-square w-[170px] mb-8" alt="">
          <h1 class="text-2xl text-neutral-900 text-bold text-left mb-5">Build</h1>
          <p class="text-base text-neutral-900/80 text-regular text-left">Deploy your own blockchain in minutes, as
            easily as a smart contract</p>
        </div>
        <div
          class="col-span-4 md:col-span-1 py-[35px] px-[25px] flex flex-col backdrop-blur-md shadow-lg w-full  rounded-md transition-all hover:shadow-2xl">
          <img src="./assets/advantage-2.png" class="aspect-square w-[170px] mb-8" alt="">
          <h1 class="text-2xl text-neutral-900 text-bold text-left mb-5">Scale</h1>
          <p class="text-base text-neutral-900/80 text-regular text-left">Access the dynamic scaling unlocked by data
            availability sampling, where scale increases with the number of users</p>
        </div>
        <div
          class="col-span-4 md:col-span-1 py-[35px] px-[25px] flex flex-col backdrop-blur-md shadow-lg w-full rounded-md transition-all hover:shadow-2xl">
          <img src="./assets/advantage-3.png" class="aspect-square w-[170px] mb-8" alt="">
          <h1 class="text-2xl text-neutral-900 text-bold text-left mb-5">Customize</h1>
          <p class="text-base text-neutral-900/80 text-regular text-left">Create applications using your favorite VM
            or define your own</p>
        </div>
        <div
          class="col-span-4 md:col-span-1 py-[35px] px-[25px] flex flex-col backdrop-blur-md shadow-lg w-full  rounded-md transition-all hover:shadow-2xl">
          <img src="./assets/advantage-4.png" class="aspect-square w-[170px] mb-8" alt="">
          <h1 class="text-2xl text-neutral-900 text-bold text-left mb-5">Sovereign</h1>
          <p class="text-base text-neutral-900/80 text-regular text-left">Build sovereign rollups, a new type of
            self-governing blockchain with minimal platform risk</p>
        </div>
      </div>
    </section>
    <section class="container mx-auto bg-fixed mt-20 px-4 lg:px-0">
      <div class="grid grid-cols-2 gap-6 lg:gap-12">
        <div class="p-8 lg:p-16 backdrop-blur-md shadow-xl col-span-2 lg:col-span-1 border rounded-md overflow-hidden">
          <div
            class="w-56 aspect-square rotate-12 bg-emerald-400/50 rounded-full mb-8 blur-3xl -bottom-32 -z-10 -right-20 absolute">
          </div>

          <h1 class="lg:text-3xl text-xl text-neutral-900 text-bold text-left ">Lorem, ipsum dolor</h1>
          <p class="mt-4 text-neutral-900/80 text-regular">Lorem, ipsum dolor sit amet consectetur adipisicing
            elit. Itaque, quae magni id consequatur repellendus exercitationem</p>
          <button
            class="mt-8 bg-emerald-500 hover:bg-emerald-600 text-white text-regular text-lg lg:py-4 lg:px-8 px-4 py-2 rounded-md">View
            Dosc</button>
        </div>
        <div class="p-8 lg:p-16 backdrop-blur-md shadow-xl col-span-2 lg:col-span-1 border rounded-md overflow-hidden">
          <div
            class="w-56 aspect-square rotate-12 bg-emerald-400/50 rounded-full mb-8 blur-3xl -bottom-32 -z-10 -right-20 absolute">
          </div>
          <h1 class="lg:text-3xl text-xl text-neutral-900 text-bold text-left ">Lorem ipsum dolor sit</h1>
          <p class="mt-4 text-neutral-900/80 text-regular">Lorem ipsum dolor, sit amet consectetur adipisicing
            elit. Delectus, minus necessitatibus nulla quis distinctio tempora veniam</p>
          <button
            class="mt-8 bg-emerald-500 hover:bg-emerald-600 text-white text-regular lg:text-lg lg:py-4 lg:px-8 px-4 py-2 rounded-md">Visit
            Rapid</button>
        </div>
        <div
          class="p-8 lg:p-16 backdrop-blur-md shadow-xl flex flex-col justify-center items-center col-span-2 border rounded-md overflow-hidden">
          <div class="w-40 h-96 rotate-12 -z-10 bg-emerald-400/50 rounded-full mb-8 blur-3xl -top-25 -left-16 absolute">
          </div>
          <div class="w-40 h-96 rotate-12 -z-10 bg-emerald-400/50 rounded-full mb-8 blur-3xl -top-25 -right-16 absolute">
          </div>
          <h1 class="text-3xl text-neutral-900 text-bold text-left ">Lorem ipsum dolor sit amet</h1>
          <p class="mt-4 text-neutral-900/80 text-regular text-normal w-full  lg:w-2/3">Lorem ipsum dolor sit amet consectetur
            adipisicing elit. Iste necessitatibus animi rem unde, non vitae dolorum odio suscipit reprehenderit, possimus
            nobis sed, harum molestias.</p>
          <button
            class="mt-8 bg-emerald-500 hover:bg-emerald-600 text-white text-regular text-lg lg:py-4 lg:px-8 px-4 py-2 rounded-md w-max">Visit
            Rapid</button>
        </div>
      </div>
    </section>
    <section class="container mx-auto bg-fixed mt-20 px-4 lg:px-0">
      <h1 class="w-full text-center text-3xl text-neutral-900 text-bold">Be Part of the Community</h1>
      <div class="grid grid-cols-3 gap-8 my-16">
        <div class="flex flex-col col-span-3 lg:col-span-1 justify-center items-center">
          <Icon icon="carbon:logo-twitter" class="text-6xl text-emerald-500" />
          <h1 class="text-2xl text-neutral-900 text-bold text-center mt-8">Twitter</h1>
          <p class="text-base text-neutral-900/80 text-regular text-center mt-4">Lorem ipsum dolor sit amet consectetur
            adipisicing elit. Iste necessitatibus animi rem unde, non vitae dolorum odio suscipit reprehenderit, possimus
            nobis sed, harum molestias.</p>
        </div>
        <div class="flex flex-col col-span-3 lg:col-span-1 justify-center items-center">
          <Icon icon="bx:bxl-discord" class="text-6xl text-emerald-500" />
          <h1 class="text-2xl text-neutral-900 text-bold text-center mt-8">Discord</h1>
          <p class="text-base text-neutral-900/80 text-regular text-center mt-4">Lorem ipsum dolor sit amet consectetur
            adipisicing elit. Iste necessitatibus animi rem unde, non vitae dolorum odio suscipit reprehenderit, possimus
            nobis sed, harum molestias.</p>
        </div>
        <div class="flex flex-col col-span-3 lg:col-span-1 justify-center items-center">
          <Icon icon="simple-icons:opensea" class="text-6xl text-emerald-500" />
          <h1 class="text-2xl text-neutral-900 text-bold text-center mt-8">Opensea</h1>
          <p class="text-base text-neutral-900/80 text-regular text-center mt-4">Lorem ipsum dolor sit amet consectetur
            adipisicing elit. Iste necessitatibus animi rem unde, non vitae dolorum odio suscipit reprehenderit, possimus
            nobis sed, harum molestias.</p>
        </div>
      </div>
    </section>
    <section id="roadMap" class="container mx-auto bg-fixed mt-20 px-4 lg:px-0">
      <h1 class="text-6xl text-neutral-900 text-bold text-left">Roadmap</h1>
      <div class="grid grid-cols-4">
        <div class="flex flex-col lg:col-span-1 col-span-4 gap-8 w-full mt-16 p-4 border-r-2">
          <div
            class="w-full border-2 flex flex-row justify-center border-emerald-500 text-center text-regular text-4xl py-4">
            <p class="text-semibold text-emerald-500">Q1</p>&nbsp;2023
          </div>
          <div class="flex flex-col gap-2">
            <Icon icon="mingcute:announcement-line" class="text-4xl text-neutral-700" />
            <div class="flex flex-row">
              <p class="text-regular text-lg">Prop 72 Passed&nbsp;<span
                  class="bg-black/10 w-max px-4 py-1 rounded-full text-regular text-lg"><span
                    class="text-emerald-500">●</span>&nbsp;Done</span></p>
            </div>
          </div>
          <div class="flex flex-col gap-2">
            <Icon icon="clarity:users-line" class="text-4xl text-neutral-700" />
            <div class="flex flex-row">
              <p class="text-regular text-lg">Basic Interchain <br> Accounts support for <br>CosmWasm&nbsp;<span
                  class="bg-black/10 w-max px-4 py-1 rounded-full text-regular text-lg"><span
                    class="text-blue-500">●</span>&nbsp;In Progress</span></p>
            </div>
          </div>
          <div class="flex flex-col gap-2">
            <Icon icon="solar:share-outline" class="text-4xl text-neutral-700" />
            <div class="flex flex-row">
              <p class="text-regular text-lg">Basic Interchain <br> Queries support for <br>CosmWasm&nbsp;<span
                  class="bg-black/10 w-max px-4 py-1 rounded-full text-regular text-lg"><span
                    class="text-blue-500">●</span>&nbsp;In Progress</span></p>
            </div>
          </div>
          <div class="flex flex-col gap-2">
            <Icon icon="wpf:statistics" class="text-4xl text-neutral-700" />
            <div class="flex flex-row">
              <p class="text-regular text-lg">Audit&nbsp;<span
                  class="bg-black/10 w-max px-4 py-1 rounded-full text-regular text-lg"><span
                    class="text-blue-500">●</span>&nbsp;In Progress</span></p>
            </div>
          </div>
        </div>
        <div class="flex flex-col gap-8 w-full lg:col-span-1 col-span-4 mt-16 p-4 border-r-2">
          <div
            class="w-full border-2 flex flex-row justify-center border-emerald-500 text-center text-regular text-4xl py-4">
            <p class="text-semibold text-emerald-500">Q1 </p>&nbsp;2023
          </div>
          <div class="flex flex-col gap-2">
            <Icon icon="carbon:network-2" class="text-4xl text-neutral-700" />
            <div class="flex flex-row">
              <p class="text-regular text-lg">Quark (Experimental) <br> Testnet</p>
            </div>
          </div>
          <div class="flex flex-col gap-2">
            <Icon icon="solar:atom-outline" class="text-4xl text-neutral-700" />
            <div class="flex flex-row">
              <p class="text-regular text-lg">Audit Report & Fixes</p>
            </div>
          </div>
          <div class="flex flex-col gap-2">
            <Icon icon="iconoir:network" class="text-4xl text-neutral-700" />
            <div class="flex flex-row">
              <p class="text-regular text-lg">Hadron (Improved) <br> Testnet</p>
            </div>
          </div>
          <div class="flex flex-col gap-2">
            <Icon icon="ph:code" class="text-4xl text-neutral-700" />
            <div class="flex flex-row">
              <p class="text-regular text-lg">Developer Onboarding</p>
            </div>
          </div>
        </div>
        <div class="flex flex-col gap-8 w-full lg:col-span-1 col-span-4 mt-16 p-4 border-r-2">
          <div
            class="w-full border-2 flex flex-row justify-center border-emerald-500 text-center text-regular text-4xl py-4">
            <p class="text-semibold text-emerald-500">Q1</p>&nbsp;2023
          </div>
          <div class="flex flex-col gap-2">
            <Icon icon="lucide:network" class="text-4xl text-neutral-700" />
            <div class="flex flex-row">
              <p class="text-regular text-lg">Baryon (Interchain-Secured) <br> Testnet</p>
            </div>
          </div>
          <div class="flex flex-col gap-2">
            <Icon icon="ph:users-four" class="text-4xl text-neutral-700" />
            <div class="flex flex-row">
              <p class="text-regular text-lg">Community Onboarding</p>
            </div>
          </div>
          <div class="flex flex-col gap-2">
            <Icon icon="charm:rocket" class="text-4xl text-neutral-700" />
            <div class="flex flex-row">
              <p class="text-regular text-lg">Interchain-secured <br> Mainnet Launch</p>
            </div>
          </div>
          <div class="flex flex-col gap-2">
            <Icon icon="mdi:stars-outline" class="text-4xl text-neutral-700" />
            <div class="flex flex-row">
              <p class="text-regular text-lg">RAPID Cahin <br> Generation Event</p>
            </div>
          </div>
          <div class="flex flex-col gap-2">
            <Icon icon="akar-icons:statistic-up" class="text-4xl text-neutral-700" />
            <div class="flex flex-row">
              <p class="text-regular text-lg">Liquidity Mining Gauges</p>
            </div>
          </div>
        </div>
        <div class="flex flex-col gap-8 w-full lg:col-span-1 col-span-4 mt-16 p-4">
          <div
            class="w-full border-2 flex flex-row justify-center border-emerald-500 text-center text-regular text-4xl py-4">
            <p class="text-semibold text-emerald-500">Q1</p>&nbsp;2023
          </div>
          <div class="flex flex-col gap-2">
            <Icon icon="lucide:network" class="text-4xl text-neutral-700" />
            <div class="flex flex-row">
              <p class="text-regular text-lg">Baryon (Interchain-Secured) <br> Testnet</p>
            </div>
          </div>
          <div class="flex flex-col gap-2">
            <Icon icon="ph:users-four" class="text-4xl text-neutral-700" />
            <div class="flex flex-row">
              <p class="text-regular text-lg">Community Onboarding</p>
            </div>
          </div>
          <div class="flex flex-col gap-2">
            <Icon icon="charm:rocket" class="text-4xl text-neutral-700" />
            <div class="flex flex-row">
              <p class="text-regular text-lg">Interchain-secured <br> Mainnet Launch</p>
            </div>
          </div>
          <div class="flex flex-col gap-2">
            <Icon icon="mdi:stars-outline" class="text-4xl text-neutral-700" />
            <div class="flex flex-row">
              <p class="text-regular text-lg">RAPID Cahin <br> Generation Event</p>
            </div>
          </div>
          <div class="flex flex-col gap-2">
            <Icon icon="akar-icons:statistic-up" class="text-4xl text-neutral-700" />
            <div class="flex flex-row">
              <p class="text-regular text-lg">Liquidity Mining Gauges</p>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section id="whoAreWe" class="container mx-auto bg-fixed my-20 px-4 lg:px-0">
      <h1 class="text-5xl text-center text-neutral-700 font-semibold">Who Are We?</h1>
      <div class="grid grid-cols-6 mt-16 gap-8">
        <div
          class="col-span-3 lg:col-span-1 py-[35px] px-[25px] flex flex-col backdrop-blur-md shadow-lg w-full rounded-md transition-all hover:shadow-2xl"
          v-for="i in 12" key="i">
          <img src="https://avatars.githubusercontent.com/u/25180623?v=4" alt="Avatar"
            class="rounded-full mx-auto w-32 h-32">
          <div class="flex flex-col gap-2 mt-4">
            <p class="text-2xl text-center text-neutral-700 font-semibold">Rahul Sethuram</p>
            <p class="text-center text-neutral-700 font-semibold">Founder & CEO</p>
          </div>
        </div>
      </div>
    </section>
    <section class="px-4 lg:px-0">
      <!--Footer-->
      <footer class="w-full bg-white text-white">
        <div class="mx-auto px-8">
          <div class="flex flex-col-reverse lg:flex-row justify-between">
            <div class="py-6 flex flex-row gap-4 w-full justify-center lg:justify-start lg:w-72">
              <img src="./assets/logo.png" alt="Logo" class="w-8 h-8 aspect-square">
              <h1 class="text-xl text-neutral-700 font-bold">RapidChain</h1>
            </div>
            <div class="py-6">
              <p class="mb-6 text-sm text-center text-neutral-700 font-bold">
                © 2021 RapidChain. All rights reserved.
              </p>
            </div>
            <div class="py-6 w-72 hidden lg:flex justify-end">
              <p class="mb-6 text-sm text-center flex flex-row gap-4 text-neutral-700 font-bold">
                <a href="" target="_blank" rel="noopener noreferrer">
                  <Icon icon="akar-icons:twitter-fill" class="text-4xl text-neutral-700" />
                </a>
                <a href="" target="_blank" rel="noopener noreferrer">
                  <Icon icon="bx:bxl-discord" class="text-4xl text-neutral-700" />
                </a>
                <a href="" target="_blank" rel="noopener noreferrer">
                  <Icon icon="simple-icons:opensea" class="text-4xl text-neutral-700" />
                </a>
              </p>
            </div>
          </div>
        </div>
      </footer>
    </section>
  </div>
</template>

<script setup>
import { Icon } from '@iconify/vue';
import { ref } from 'vue';

const aside = ref(false);
</script>