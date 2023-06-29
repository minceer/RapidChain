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
              <a class="text-xl hover:text-green-600 text-gray-600 text-regular" href="#adventage">Rapid_</a>
              <a class="text-xl hover:text-green-600 text-gray-600 text-regular" href="#roadMap">Roadmap</a>
            </div>
          </div>
        </div>
        <div class="hidden md:flex gap-10 h-max my-auto">
          <a class="text-xl hover:text-green-600 text-gray-600 text-regular" href="#home">Home</a>
          <a class="text-xl hover:text-green-600 text-gray-600 text-regular" href="#adventage">Rapid_</a>
          <a class="text-xl hover:text-green-600 text-gray-600 text-regular" href="#roadMap">Roadmap</a>
        </div>
      </div>
    </div>
    <section id="home" class="container mx-auto bg-fixed 2xl:px-0 pt-20 px-4 lg:px-0">
      <div class="w-full flex flex-col-reverse md:flex-row gap-2">
        <div class="flex flex-col relative w-full z-20">
          <p class="text-neutral-900 text-4xl md:text-[110px] md:leading-[106px] text-bold mt-20">First user-oriented  <br
              class="md:block hidden"> Blockchain <br class="md:block hidden"> Network</p>
          <p class="mt-4 text-neutral-900/80 md:mt-16 text-regular text-normal md:text-xl">Experience the Power of RapidChain: <br class="md:block hidden"> A Blockchain
That's Fast, Secure, Affordable, and Packed with
Advanced Features.</p>
        </div>
      
      </div>
    </section>
    <section id="adventage" class="container mx-auto bg-fixed mt-20 px-4 lg:px-0">
      <h1 class="lg:text-7xl text-4xl text-neutral-900 text-bold text-left">Rapid_</h1>
      <div class="grid grid-cols-4 gap-2 mt-10">
        <div
          class="col-span-4 md:col-span-1 py-[35px] px-[25px] flex flex-col backdrop-blur-md shadow-lg w-full rounded-md transition-all hover:shadow-2xl">
          <img src="./assets/deadline.png" class="aspect-square w-[170px] mb-8" alt="">
          <h1 class="text-2xl text-neutral-900 text-bold text-left mb-5">Speed_</h1>
          <p class="text-base text-neutral-900/80 text-regular text-left">Experience instant
transactions</p>
        </div>
        <div
          class="col-span-4 md:col-span-1 py-[35px] px-[25px] flex flex-col backdrop-blur-md shadow-lg w-full  rounded-md transition-all hover:shadow-2xl">
          <img src="./assets/encrypted.png" class="aspect-square w-[170px] mb-8" alt="">
          <h1 class="text-2xl text-neutral-900 text-bold text-left mb-5">Security</h1>
          <p class="text-base text-neutral-900/80 text-regular text-left">
Advanced security
measures to safeguard
your digital assets.</p>
        </div>
        <div
          class="col-span-4 md:col-span-1 py-[35px] px-[25px] flex flex-col backdrop-blur-md shadow-lg w-full rounded-md transition-all hover:shadow-2xl">
          <img src="./assets/energy-control.png" class="aspect-square w-[170px] mb-8" alt="">
          <h1 class="text-2xl text-neutral-900 text-bold text-left mb-5">Cost-Efficiency</h1>
          <p class="text-base text-neutral-900/80 text-regular text-left">Reduce transaction fees
and operational costs
with $RAPID</p>
        </div>
        
      </div>
    </section>
    <section class="container mx-auto bg-fixed mt-20 px-4 lg:px-0">
      <div class="grid grid-cols-2 gap-6 lg:gap-12">
        <div class="p-8 lg:p-16 backdrop-blur-md shadow-xl col-span-2 lg:col-span-1 border rounded-md overflow-hidden">
          <div
            class="w-56 aspect-square rotate-12 bg-emerald-400/50 rounded-full mb-8 blur-3xl -bottom-32 -z-10 -right-20 absolute">
          </div>

          <h1 class="lg:text-3xl text-xl text-neutral-900 text-bold text-left ">Lets Build</h1>
          <p class="mt-4 text-neutral-900/80 text-regular">For individuals and teams who are keen on building innovative projects utilizing Rapidchain and are in search of comprehensive insights into the network’s technical nuances and specifications</p>
          <button
            class="mt-8 bg-emerald-500 hover:bg-emerald-600 text-white text-regular text-lg lg:py-4 lg:px-8 px-4 py-2 rounded-md">View
            Docs</button>
        </div>
        <div class="p-8 lg:p-16 backdrop-blur-md shadow-xl col-span-2 lg:col-span-1 border rounded-md overflow-hidden">
          <div
            class="w-56 aspect-square rotate-12 bg-emerald-400/50 rounded-full mb-8 blur-3xl -bottom-32 -z-10 -right-20 absolute">
          </div>
          <h1 class="lg:text-3xl text-xl text-neutral-900 text-bold text-left ">$RAPID</h1>
          <p class="mt-4 text-neutral-900/80 text-regular">For individuals and entities interested in acquiring $RAPID tokens and actively contributing to the advancement and success of the project</p>
          <button
            class="mt-8 bg-emerald-500 hover:bg-emerald-600 text-white text-regular lg:text-lg lg:py-4 lg:px-8 px-4 py-2 rounded-md">Get $RAPID</button>
        </div>
        <div
          class="p-8 lg:p-16 backdrop-blur-md shadow-xl flex flex-col justify-center items-center col-span-2 border rounded-md overflow-hidden">
          <div class="w-40 h-96 rotate-12 -z-10 bg-emerald-400/50 rounded-full mb-8 blur-3xl -top-25 -left-16 absolute">
          </div>
          <div class="w-40 h-96 rotate-12 -z-10 bg-emerald-400/50 rounded-full mb-8 blur-3xl -top-25 -right-16 absolute">
          </div>
          <h1 class="text-3xl text-neutral-900 text-bold text-left ">Partnership & Investment</h1>
          <p class="mt-4 text-neutral-900/80 text-regular text-normal w-full  lg:w-2/3">For individuals and organizations seeking comprehensive insights into strategic partnerships, corporate investment opportunities, and collaborative endeavors.</p>
          <button
            class="mt-8 bg-emerald-500 hover:bg-emerald-600 text-white text-regular text-lg lg:py-4 lg:px-8 px-4 py-2 rounded-md w-max">Get Contact</button>
        </div>
      </div>
    </section>
    <section class="container mx-auto bg-fixed mt-20 px-4 lg:px-0">
      <h1 class="w-full text-center text-3xl text-neutral-900 text-bold">Be Part of the Community</h1>
      <div class="grid grid-cols-3 gap-8 my-16">
        <div class="flex flex-col col-span-3 lg:col-span-1 justify-center items-center">
          <Icon icon="carbon:logo-twitter" class="text-6xl text-emerald-500" />
          <h1 class="text-2xl text-neutral-900 text-bold text-center mt-8">Twitter</h1>
          <p class="text-base text-neutral-900/80 text-regular text-center mt-4">Follow us on Twitter for news, announcements, and
At Rapidchain, we believe in the community interaction.</p>
        </div>
        <div class="flex flex-col col-span-3 lg:col-span-1 justify-center items-center">
          <Icon icon="simple-icons:telegram" class="text-6xl text-emerald-500" />
          <h1 class="text-2xl text-neutral-900 text-bold text-center mt-8">Telegram</h1>
          <p class="text-base text-neutral-900/80 text-regular text-center mt-4">Join our Telegram community for real-time updates, lively
Community: Join discussions, and direct access to our team.</p>
        </div>
        <div class="flex flex-col col-span-3 lg:col-span-1 justify-center items-center">
          <Icon icon="simple-icons:medium" class="text-6xl text-emerald-500" />
          <h1 class="text-2xl text-neutral-900 text-bold text-center mt-8">Medium</h1>
          <p class="text-base text-neutral-900/80 text-regular text-center mt-4">Explore our Medium publication for insightful articles and
global community of blockchain thought leadership.</p>
        </div>
      </div>
    </section>
    <section id="roadMap" class="container mx-auto bg-fixed mt-20 px-4 lg:px-0">
      <h1 class="text-6xl text-neutral-900 text-bold text-left">Roadmap</h1>
      <div class="grid grid-cols-4">
        <div class="flex flex-col lg:col-span-1 col-span-4 gap-8 w-full mt-16 p-4 border-r-2">
          <div
            class="w-full border-2 flex flex-row justify-center border-emerald-500 text-center text-regular text-4xl py-4">
            <p class="text-semibold text-emerald-500">Q2</p>&nbsp;2023
          </div>
         
         
        </div>
        <div class="flex flex-col gap-8 w-full lg:col-span-1 col-span-4 mt-16 p-4 border-r-2">
          <div
            class="w-full border-2 flex flex-row justify-center border-emerald-500 text-center text-regular text-4xl py-4">
            <p class="text-semibold text-emerald-500">Q3 </p>&nbsp;2023
          </div>
        </div>
        <div class="flex flex-col gap-8 w-full lg:col-span-1 col-span-4 mt-16 p-4 border-r-2">
          <div
            class="w-full border-2 flex flex-row justify-center border-emerald-500 text-center text-regular text-4xl py-4">
            <p class="text-semibold text-emerald-500">Q4</p>&nbsp;2023
          </div>
        </div>
        <div class="flex flex-col gap-8 w-full lg:col-span-1 col-span-4 mt-16 p-4">
          <div
            class="w-full border-2 flex flex-row justify-center border-emerald-500 text-center text-regular text-4xl py-4">
            <p class="text-semibold text-emerald-500">Q1</p>&nbsp;2024
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
                  <Icon icon="simple-icons:twitter" class="text-4xl text-neutral-700" />
                </a>
                <a href="" target="_blank" rel="noopener noreferrer">
                  <Icon icon="simple-icons:medium" class="text-4xl text-neutral-700" />
                </a>
                <a href="" target="_blank" rel="noopener noreferrer">
                  <Icon icon="simple-icons:telegram" class="text-4xl text-neutral-700" />
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