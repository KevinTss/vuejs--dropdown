<template>
  <div id="app" class="antialiased text-gray-900 flex flex-col min-h-screen bg-gray-200">
    <div class="flex justify-center items-center flex-1">
      <AppDropdown>
        <template slot="toggler">
          <button
            class="relative flex items-center focus:outline-none pl-5 pr-3 py-2 rounded-lg bg-gray-300 text-gray-800 font-semibold"
          >
            Click me
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 24 24"
              class="ml-1 h-5 w-5 fill-current text-gray-700"
            >
              <path
                d="M15.3 9.3a1 1 0 0 1 1.4 1.4l-4 4a1 1 0 0 1-1.4 0l-4-4a1 1 0 0 1 1.4-1.4l3.3 3.29 3.3-3.3z"
              ></path>
            </svg>
          </button>
        </template>
        <AppDropdownContent>
          <AppDropdownItem>Action 1</AppDropdownItem>
          <AppDropdownItem>Action 2</AppDropdownItem>
          <AppDropdownItem>Action 3</AppDropdownItem>
        </AppDropdownContent>
      </AppDropdown>
    </div>
  </div>
</template>

<script>
import AppDropdown from "./components/Dropdown.vue";
import AppDropdownContent from "./components/DropdownContent.vue";
import AppDropdownItem from "./components/DropdownItem.vue";

export default {
  name: "app",
  components: {
    AppDropdown,
    AppDropdownContent,
    AppDropdownItem
  }
};
</script>
