<template>
    <div class="flex  px-10 py-10 gap-10 ">
        <div class="w-3/5 shadow-xl">
            <H2 class="py-5 ">Recents Task</H2>
            <div v-if="userResponses == ''">
                <div class="flex flex-col justify-center items-center py-10   gap-10 ">
                    <svg class="animate-pulse" width="216" height="55" viewBox="0 0 216 45" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <rect x="0.25" y="0.25" width="215.5" height="44.5" rx="7.75" fill="#D9D9D9" fill-opacity="0.2"
                            stroke="#D9D9D9" stroke-width="0.5" />
                        <rect x="21" y="12" width="59" height="8" rx="4" fill="#F5EFEF" />
                        <rect x="21" y="29" width="166" height="9" rx="4" fill="#E9E1E1" />
                        <rect x="192" y="12" width="10" height="8" rx="4" fill="#E9E1E1" />
                        <rect x="192" y="29" width="10" height="8" rx="4" fill="#E9E1E1" />
                    </svg>
                    <H2>No Tasks Yet</H2>
                    <p class="w-1/2 text-center">Start By Adding Tasks to your board and track your progress</p>
                    <div @click="$emit('toggleDisplay')"
                        class="flex items-center justify-center bg-[#4B04A7] text-white w-[9.25rem] h-[3rem] rounded-3xl">
                        <button class="flex justify-center">
                            <span class="material-symbols-outlined"> add</span>
                            Add Task
                        </button>
                    </div>
                </div>
            </div>

            <div v-else>
                <div v-for="userResponse in userResponses">
                    <div class="flex justify-between items-center">
                        <div class="flex py-1">
                            <div>🏃</div>
                            <div class="flex flex-col w-32">
                                <span class="pb-2 "> {{ userResponse.task }}</span>
                                <span class="text-sm">{{ userResponse.date }}</span>
                            </div>
                        </div>
                        <div class="">
                            <div class="flex flex-col ">
                                <span class="pb-2"> {{ userResponse.priority }}</span>
                                <!-- Show Medium -->
                                <span v-if="userResponse.priority === 'Medium'">
                                    <svg width="194" height="6" viewBox="0 0 194 6" fill="none"
                                        xmlns="http://www.w3.org/2000/svg">
                                        <path d="M3 3H191" stroke="#FBB01E" stroke-opacity="0.1" stroke-width="5"
                                            stroke-linecap="round" />
                                        <path d="M3 3H114" stroke="#FBB01E" stroke-width="5" stroke-linecap="round" />
                                    </svg>
                                </span>
                                <!-- Show Low -->
                                <span v-else-if="userResponse.priority === 'Low'" class="w-1/3">
                                    <svg width="194" height="6" viewBox="0 0 194 6" fill="none"
                                        xmlns="http://www.w3.org/2000/svg">
                                        <path d="M3 3H191" stroke="#56EC77" stroke-opacity="0.08" stroke-width="5"
                                            stroke-linecap="round" />
                                        <path d="M3 3H48" stroke="#56EC77" stroke-width="5" stroke-linecap="round" />
                                    </svg>
                                </span>
                                <!-- Show High -->
                                <span v-else>
                                    <svg width="194" height="6" viewBox="0 0 194 6" fill="none"
                                        xmlns="http://www.w3.org/2000/svg">
                                        <path d="M3 3H191" stroke="#FF4242" stroke-opacity="0.1" stroke-width="5"
                                            stroke-linecap="round" />
                                        <path d="M3 3H191" stroke="#FF4242" stroke-width="5" stroke-linecap="round" />
                                    </svg>
                                </span>
                            </div>
                        </div>
                        <div v-if="userResponse.priority === 'Medium'">
                            <div class="flex flex-col w-12">
                                <span class="material-symbols-outlined">
                                    more_horiz
                                </span>
                                <span>50%</span>
                            </div>
                        </div>
                        <div v-else-if="userResponse.priority === 'Low'">
                            <div class="flex flex-col w-12">
                                <span class="material-symbols-outlined">
                                    more_horiz
                                </span>
                                <span>25%</span>
                            </div>
                        </div>
                        <div v-else>
                            <div class="flex flex-col w-12">
                                <span class="material-symbols-outlined">
                                    more_horiz
                                </span>
                                <span>100%</span>
                            </div>
                        </div>
                    </div>

                </div>
            </div>
        </div>

        <div class="w-3/5  py-5 p-5 shadow-xl">
            <h2>Other Commandos</h2>
            <div class="h-[40vh] overflow-y-auto">
                <div class="flex justify-between  items-center py-5">
                    <div class="flex items-center gap-5">
                        <div class="">
                            <img class="rounded-full w-10 h-10" src="https://source.unsplash.com/user/c_v_r"
                                alt="Free Images">
                        </div>
                        <p>Celestian Bean</p>
                    </div>
                    <div>
                        <span class="material-symbols-outlined">
                            navigate_next
                        </span>
                    </div>
                </div>
                <div class="flex  justify-between items-center py-5">
                    <div class="flex items-center gap-5">
                        <img class="rounded-full w-10 h-10" src="https://source.unsplash.com/user/c_v_r" alt="Free Images">
                        <span>Stephenny Bills</span>
                    </div>
                    <div>
                        <span class="material-symbols-outlined">
                            navigate_next
                        </span>
                    </div>
                </div>
                <div class="flex justify-between items-center py-5">
                    <div class="flex items-center gap-5">
                        <img class="rounded-full w-10 h-10" src="https://source.unsplash.com/user/c_v_r" alt="Free Images">
                        <span>Musky Elena</span>
                    </div>
                    <div>
                        <span class="material-symbols-outlined">
                            navigate_next
                        </span>
                    </div>
                </div>
                <div class="flex  justify-between items-center py-5 ">
                    <div class="flex items-center gap-5">
                        <img class="rounded-full w-10 h-10" src="https://source.unsplash.com/user/c_v_r" alt="Free Images">
                        <span>Jackson Benny</span>
                    </div>
                    <div>
                        <span class="material-symbols-outlined">
                            navigate_next
                        </span>
                    </div>
                </div>
                <div class="flex justify-between items-center py-5 ">
                    <div class="flex items-center gap-5">
                        <img class="rounded-full w-10 h-10" src="https://source.unsplash.com/user/c_v_r" alt="Free Images">
                        <span>John Doe</span>
                    </div>
                    <div>
                        <span class="material-symbols-outlined">
                            navigate_next
                        </span>
                    </div>
                </div>
                <div class="flex justify-between items-center py-5 ">
                    <div class="flex items-center gap-5">
                        <img class="rounded-full w-10 h-10" src="https://source.unsplash.com/user/c_v_r" alt="Free Images">
                        <span>John Doe</span>
                    </div>
                    <div>
                        <span class="material-symbols-outlined">
                            navigate_next
                        </span>
                    </div>
                </div>



            </div>

        </div>
    </div>
</template>


<script >
export default {
    name: "Tasks",
    props: ['userResponses', 'display'],
//     methods: {
//         toggleDisplay() {
//             this.$emit('toggle-display')
//     }
//  }
}
</script>

<style scoped>
/* width */
::-webkit-scrollbar {
    width: 10px;
    height: 5px;
}


/* Handle */
::-webkit-scrollbar-thumb {
    background: #4B04A7;
    border-radius: 100vh;
    border: 3px solid #4B04A7;
}

/* Handle on hover */
::-webkit-scrollbar-thumb:hover {
    background: #4B04A7;
}
</style>