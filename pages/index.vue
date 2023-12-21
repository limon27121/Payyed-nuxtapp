
<template>
    <header>
        <div class="flex">
            <div class="flex items-center pl-28 pt-10">
        <img src="~/assets/e1.png" alt="" class="pr-4">
        <a href="#" class="py-2 px-4 text-black font-bold transition duration-300 hover:text-green-600 focus:outline-none">DASHBOARD</a>
        <a href="#" class="py-2 px-4 text-black font-bold transition duration-300 hover:text-green-600 focus:outline-none">TRANSACTIONS</a>
        <a href="#" class="py-2 px-4 text-black font-bold transition duration-300 hover:text-green-600 focus:outline-none">SEND/REQUEST</a>
        <a href="#" class="py-2 px-4 text-black font-bold transition duration-300 hover:text-green-600 focus:outline-none">HELP</a>
  
        <div class="relative" @mouseover="openDropdown(1)" @mouseleave="closeDropdown(1)">
          <button class="py-2 px-4 text-black font-bold transition duration-300 hover:text-green-600 focus:outline-none">FEATURES</button>
          <div v-if="isDropdownOpen[1]" class="dropdown-content absolute bg-gray-100 shadow-md mt-2">
            <a href="#" class="block py-2 px-4 text-black no-underline hover:bg-gray-200">Link 1</a>
            <a href="#" class="block py-2 px-4 text-black no-underline hover:bg-gray-200">Link 2</a>
            <a href="#" class="block py-2 px-4 text-black no-underline hover:bg-gray-200">Link 3</a>
          </div>
        </div>
  
        <div class="relative" @mouseover="openDropdown(2)" @mouseleave="closeDropdown(2)">
          <button class="py-2 px-4 text-black font-bold transition duration-300 hover:text-green-600 focus:outline-none">PAGES</button>
          <div v-if="isDropdownOpen[2]" class="dropdown-content absolute bg-gray-100 shadow-md mt-2">
            <a href="#" class="block py-2 px-4 text-black no-underline hover:bg-gray-200">Link 1</a>
            <a href="#" class="block py-2 px-4 text-black no-underline hover:bg-gray-200">Link 2</a>
            <a href="#" class="block py-2 px-4 text-black no-underline hover:bg-gray-200">Link 3</a>
          </div>
        </div>
        <div>   
        </div>
        </div>
        <div class="pt-12 pl-40 flex">
            <div class="relative" @mouseover="openDropdown(3)" @mouseleave="closeDropdown(3)">
          <button class="py-2 px-4 text-black font-bold transition duration-300 hover:text-green-600 focus:outline-none">EN</button>
          <div v-if="isDropdownOpen[3]" class="dropdown-content absolute bg-gray-100 shadow-md mt-2">
            <a href="#" class="block py-2 px-4 text-black no-underline hover:bg-gray-200">Link 1</a>
            <a href="#" class="block py-2 px-4 text-black no-underline hover:bg-gray-200">Link 2</a>
            <a href="#" class="block py-2 px-4 text-black no-underline hover:bg-gray-200">Link 3</a>
          </div>
        </div>
        <div>
            <img src="~/assets/bell.png" class="rounded-full w-10 h-10 pl-2 ml-2" >
        </div>
        <div>
            <img src="~/assets/navlogo.png" alt="" class="rounded-full w-10 pl-2 ml-4">
        </div>
       

        </div>
        </div>
        
    </header>
    <nav class="bg-green-600 p-4 flex items-center justify-center mt-10 ">
      <a href="#" class="py-2 px-4 text-white font-bold transition duration-300 hover:text-slate-100 focus:outline-none">Account</a>
      <a href="#" class="py-2 px-4 text-white font-bold transition duration-300 hover:text-slate-100 focus:outline-none">Security</a>
      <a href="#" class="py-2 px-4 text-white font-bold transition duration-300 hover:text-slate-100 focus:outline-none">Payment Methods</a>
      <a href="#" class="py-2 px-4 text-white font-bold transition duration-300 hover:text-slate-100 focus:outline-none">Notifications</a>
    </nav>
    
  </template>
  
  <script>
  export default {
    data() {
      return {
        isDropdownOpen: { 1: false, 2: false },
      };
    },
    methods: {
      openDropdown(index) {
        this.isDropdownOpen[index] = true;
      },
      closeDropdown(index) {
        this.isDropdownOpen[index] = false;
      },
    },
  };
  </script>
  
  <style>
  /* Your global styles go here */
  </style>
  