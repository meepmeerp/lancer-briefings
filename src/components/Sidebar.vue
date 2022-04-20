<script>
import {BootstrapVue, BootstrapVueIcons} from 'bootstrap-vue'
Vue.use(BootstrapVue)
Vue.use(BootstrapVueIcons)
export default {
    data(){
        return{
        button_text: "text"
        }
    },
    methods:{
        transition(){
            this.button_text="transitioned!"
        }
    },
    components:{
        BIcon
    }
}
</script>


<template>
        <div>
  <b-button size="sm" @click="toggle">
    {{ show ? 'Hide' : 'Show' }} Alert
  </b-button>
  <b-alert
    v-model="show"
    class="mt-3"
    dismissible
    @dismissed="dismissed"
  >
    Hello World!
  </b-alert>
</div>
</template>
