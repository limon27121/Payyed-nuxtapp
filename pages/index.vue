
<template>
    <header>
        <div class="flex">
            <div class="flex items-center pl-28 pt-10">
        <img src="~/assets/e1.png" alt="" class="pr-4">
        <a href="#" class="py-2 px-4 text-black font-bold hover:bg-green-600">DASHBOARD</a>
        <a href="#" class="py-2 px-4 text-black font-bold hover:bg-green-600">TRANSACTIONS</a>
        <a href="#" class="py-2 px-4 text-black font-bold hover:bg-green-600">SEND/REQUEST</a>
        <a href="#" class="py-2 px-4 text-black font-bold hover:bg-green-600">HELP</a>
  
        <div class="relative" @mouseover="openDropdown(1)" @mouseleave="closeDropdown(1)">
          <button class="py-2 px-4 text-black no-underline hover:underline font-bold hover:bg-green-600">FEATURES</button>
          <div v-if="isDropdownOpen[1]" class="dropdown-content absolute bg-gray-100 shadow-md mt-2">
            <a href="#" class="block py-2 px-4 text-black no-underline hover:bg-gray-200">Link 1</a>
            <a href="#" class="block py-2 px-4 text-black no-underline hover:bg-gray-200">Link 2</a>
            <a href="#" class="block py-2 px-4 text-black no-underline hover:bg-gray-200">Link 3</a>
          </div>
        </div>
  
        <div class="relative" @mouseover="openDropdown(2)" @mouseleave="closeDropdown(2)">
          <button class="py-2 px-4 text-black no-underline hover:underline font-bold hover:bg-green-600">PAGES</button>
          <div v-if="isDropdownOpen[2]" class="dropdown-content absolute bg-gray-100 shadow-md mt-2">
            <a href="#" class="block py-2 px-4 text-black no-underline hover:bg-gray-200">Link 1</a>
            <a href="#" class="block py-2 px-4 text-black no-underline hover:bg-gray-200">Link 2</a>
            <a href="#" class="block py-2 px-4 text-black no-underline hover:bg-gray-200">Link 3</a>
          </div>
        </div>
        <div>   
        </div>
        </div>
        <div class="pt-12 pl-40">
            <div class="relative" @mouseover="openDropdown(3)" @mouseleave="closeDropdown(3)">
          <button class="py-2 px-4 text-black no-underline hover:underline font-bold hover:bg-green-600">EN</button>
          <div v-if="isDropdownOpen[3]" class="dropdown-content absolute bg-gray-100 shadow-md mt-2">
            <a href="#" class="block py-2 px-4 text-black no-underline hover:bg-gray-200">Link 1</a>
            <a href="#" class="block py-2 px-4 text-black no-underline hover:bg-gray-200">Link 2</a>
            <a href="#" class="block py-2 px-4 text-black no-underline hover:bg-gray-200">Link 3</a>
          </div>
        </div>
        
        </div>
        </div>
        
    </header>
    <nav class="bg-green-600 p-4 flex items-center justify-center mt-10 ">
      <a href="#" class="mx-4 text-black hover:bg-slate-400 text-slate-100 font-medium">Account</a>
      <a href="#" class="mx-4 text-black hover:bg-slate-400 text-slate-100 font-medium">Security</a>
      <a href="#" class="mx-4 text-black hover:bg-slate-400 text-slate-100 font-medium">Payment Methods</a>
      <a href="#" class="mx-4 text-black hover:bg-slate-400 text-slate-100 font-medium">Notifications</a>
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
  