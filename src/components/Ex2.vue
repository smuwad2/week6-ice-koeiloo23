<script>
    export default { 
        data() {
            return {
                width: '200',
                height: '200',
                myImg: '/assets/me.png'
            }
        },
    }
</script>

<template>

    <!-- add code here -->
    <div id="photo">
        <img v-bind:src="myImg" v-bind:width="width" v-bind:height="height"> 
        <!-- : is a short hand notation for v-bind -->
    </div>
   
</template>
