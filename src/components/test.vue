<style>
.test{
    display:block;
    width:100px;
    height: 40px;
    margin:100px auto 0;
    background-color:#ddd;
    border-radius:6px;
    border:none;
    cursor:pointer;
    outline:none;
}
</style>

<template>
    <div id="test">
        <button class="test" @click="test">点击看看</button>
    </div>
</template>


<script>
import bus from '../../static/js/bus'
export default {
    data () {
        return {
            name:"limingru"
        }
    },
    methods:{
        test () {
            bus.$emit('test', this.name)
        }
    } 
}
</script>



