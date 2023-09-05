<template>
    <section >

       <NavBar />

        <aside id="logo-sidebar"
            class="fixed top-0 left-0 z-40 w-64 h-screen pt-20 transition-transform -translate-x-full bg-white border-r border-gray-200 sm:translate-x-0 "
            aria-label="Sidebar">
            
            <div class="h-full px-3 pb-4 overflow-y-auto bg-white my-5">
                <ul class="space-y-2 font-medium">
                    <li>
                        <a href="#"
                            class="flex items-center p-2 text-gray-900 rounded-lg  hover:bg-gray-100  group">
                            <svg class="w-5 h-5 text-gray-500 transition duration-75 dark:text-gray-400 group-hover:text-gray-900 dark:group-hover:text-white"
                                aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="currentColor"
                                viewBox="0 0 22 21">
                                <path
                                    d="M16.975 11H10V4.025a1 1 0 0 0-1.066-.998 8.5 8.5 0 1 0 9.039 9.039.999.999 0 0 0-1-1.066h.002Z" />
                                <path
                                    d="M12.5 0c-.157 0-.311.01-.565.027A1 1 0 0 0 11 1.02V10h8.975a1 1 0 0 0 1-.935c.013-.188.028-.374.028-.565A8.51 8.51 0 0 0 12.5 0Z" />
                            </svg>
                            <span class="ml-3">Dashboard</span>
                        </a>
                    </li>
                    <li>
                        <a href="#"
                            class="flex items-center p-2 text-gray-900 rounded-lg  hover:bg-gray-100 dark:hover:bg-gray-700 group">
                            <svg class="flex-shrink-0 w-5 h-5 text-gray-500 transition duration-75 dark:text-gray-400 group-hover:text-gray-900 dark:group-hover:text-white"
                                width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <path fill-rule="evenodd" clip-rule="evenodd"
                                    d="M10 18C12.1217 18 14.1566 17.1571 15.6569 15.6569C17.1571 14.1566 18 12.1217 18 10C18 7.87827 17.1571 5.84344 15.6569 4.34315C14.1566 2.84285 12.1217 2 10 2C7.87827 2 5.84344 2.84285 4.34315 4.34315C2.84285 5.84344 2 7.87827 2 10C2 12.1217 2.84285 14.1566 4.34315 15.6569C5.84344 17.1571 7.87827 18 10 18ZM9.555 7.168C9.4044 7.06752 9.22935 7.00981 9.04852 7.00103C8.86769 6.99224 8.68786 7.03272 8.52823 7.11813C8.3686 7.20354 8.23516 7.33068 8.14213 7.48599C8.04909 7.6413 7.99997 7.81896 8 8V12C7.99997 12.181 8.04909 12.3587 8.14213 12.514C8.23516 12.6693 8.3686 12.7965 8.52823 12.8819C8.68786 12.9673 8.86769 13.0078 9.04852 12.999C9.22935 12.9902 9.4044 12.9325 9.555 12.832L12.555 10.832C12.692 10.7407 12.8043 10.617 12.8819 10.4718C12.9596 10.3267 13.0002 10.1646 13.0002 10C13.0002 9.83539 12.9596 9.67332 12.8819 9.52818C12.8043 9.38304 12.692 9.25932 12.555 9.168L9.555 7.168Z"
                                    fill="#999999" />
                            </svg>

                            <span class="flex-1 ml-3 whitespace-nowrap">Media</span>
                        </a>
                    </li>
                    <li>
                        <a href="#"
                            class="flex items-center p-2 text-gray-900 rounded-lg  hover:bg-gray-100 dark:hover:bg-gray-700 group">
                            <svg class="flex-shrink-0 w-5 h-5 text-gray-500 transition duration-75 dark:text-gray-400 group-hover:text-gray-900 dark:group-hover:text-white"
                                width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <g id="Mail">
                                    <path id="Vector"
                                        d="M2.00293 5.884L9.99993 9.882L17.9969 5.884C17.9673 5.37444 17.744 4.89549 17.3728 4.54523C17.0015 4.19497 16.5103 3.99991 15.9999 4H3.99993C3.48951 3.99991 2.99838 4.19497 2.62711 4.54523C2.25584 4.89549 2.03253 5.37444 2.00293 5.884Z"
                                        fill="#999999" />
                                    <path id="Vector_2"
                                        d="M18 8.11816L10 12.1182L2 8.11816V14.0002C2 14.5306 2.21071 15.0393 2.58579 15.4144C2.96086 15.7895 3.46957 16.0002 4 16.0002H16C16.5304 16.0002 17.0391 15.7895 17.4142 15.4144C17.7893 15.0393 18 14.5306 18 14.0002V8.11816Z"
                                        fill="#999999" />
                                </g>
                            </svg>

                            <span class="flex-1 ml-3 whitespace-nowrap">Chat</span>
                            <span
                                class="inline-flex items-center justify-center w-3 h-3 p-3 ml-3 text-sm font-medium text-white bg-[#4B04A7] rounded-full ">3</span>
                        </a>
                    </li>
                    <li>
                        <a href="#"
                            class="flex items-center p-2 text-gray-900 rounded-lg  hover:bg-gray-100 dark:hover:bg-gray-700 group">
                            <svg class="flex-shrink-0 w-5 h-5 text-gray-500 transition duration-75 dark:text-gray-400 group-hover:text-gray-900 dark:group-hover:text-white"
                                width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <path fill-rule="evenodd" clip-rule="evenodd"
                                    d="M13.7881 3.8039C13.3321 1.9319 10.6681 1.9319 10.2121 3.8039C10.144 4.0852 10.0105 4.34645 9.82236 4.5664C9.63424 4.78634 9.39685 4.95876 9.1295 5.06963C8.86216 5.18049 8.57242 5.22667 8.28385 5.20441C7.99529 5.18215 7.71606 5.09207 7.46889 4.9415C5.82249 3.9383 3.93849 5.8223 4.94169 7.4687C5.58969 8.5319 5.01489 9.9191 3.80529 10.2131C1.93209 10.6679 1.93209 13.3331 3.80529 13.7867C4.08666 13.8549 4.34796 13.9885 4.5679 14.1768C4.78785 14.3651 4.96022 14.6026 5.07098 14.8701C5.18174 15.1376 5.22776 15.4274 5.20529 15.7161C5.18283 16.0047 5.09251 16.284 4.94169 16.5311C3.93849 18.1775 5.82249 20.0615 7.46889 19.0583C7.71602 18.9075 7.99527 18.8172 8.28391 18.7947C8.57255 18.7722 8.86242 18.8183 9.12991 18.929C9.39739 19.0398 9.63494 19.2121 9.8232 19.4321C10.0115 19.652 10.1451 19.9133 10.2133 20.1947C10.6681 22.0679 13.3333 22.0679 13.7869 20.1947C13.8553 19.9135 13.9891 19.6524 14.1774 19.4326C14.3657 19.2128 14.6032 19.0405 14.8706 18.9298C15.138 18.8191 15.4278 18.773 15.7163 18.7953C16.0049 18.8176 16.2841 18.9078 16.5313 19.0583C18.1777 20.0615 20.0617 18.1775 19.0585 16.5311C18.9079 16.2839 18.8178 16.0047 18.7955 15.7161C18.7732 15.4276 18.8192 15.1378 18.93 14.8704C19.0407 14.603 19.213 14.3655 19.4328 14.1772C19.6525 13.9889 19.9137 13.8551 20.1949 13.7867C22.0681 13.3319 22.0681 10.6667 20.1949 10.2131C19.9135 10.1449 19.6522 10.0113 19.4323 9.82302C19.2123 9.63475 19.04 9.39721 18.9292 9.12972C18.8184 8.86223 18.7724 8.57236 18.7949 8.28372C18.8174 7.99508 18.9077 7.71583 19.0585 7.4687C20.0617 5.8223 18.1777 3.9383 16.5313 4.9415C16.2842 5.09232 16.0049 5.18264 15.7163 5.20511C15.4276 5.22757 15.1378 5.18155 14.8703 5.07079C14.6028 4.96003 14.3652 4.78766 14.177 4.56772C13.9887 4.34777 13.8551 4.08648 13.7869 3.8051L13.7881 3.8039ZM12.0001 15.5999C12.9549 15.5999 13.8705 15.2206 14.5457 14.5455C15.2208 13.8704 15.6001 12.9547 15.6001 11.9999C15.6001 11.0451 15.2208 10.1294 14.5457 9.45432C13.8705 8.77919 12.9549 8.3999 12.0001 8.3999C11.0453 8.3999 10.1296 8.77919 9.45451 9.45432C8.77938 10.1294 8.40009 11.0451 8.40009 11.9999C8.40009 12.9547 8.77938 13.8704 9.45451 14.5455C10.1296 15.2206 11.0453 15.5999 12.0001 15.5999Z"
                                    fill="#999999" />
                            </svg>
                            <span class="flex-1 ml-3 whitespace-nowrap">Settings</span>
                        </a>
                    </li>
                </ul>
            </div>
        </aside>

        <Dashboard />

    </section>
</template>







<script setup>
import NavBar from './NavBar.vue';
import Dashboard from '../Pages/Dashboard.vue'
</script>




<style lang="scss" scoped></style>