<template>
    <div>
        <app-header/>
        <div class="container">
       
            <UserProfile 
              :alsoKnownAs="data.name"
                lastname="Jones"/>
            
        </div>

    </div>
</template>

<script setup>

    import UserProfile from './components/User/Profile.vue';
    
     import { reactive } from 'vue';

     const data =reactive({
        name:'Francis'
     })


</script>
<style>
    body {
        padding: 0;
        margin: 0;
        font-family: 'Robot',sans-serif;
    }
    .container {
        min-height:84vh;
        box-sizing: border-box;
        padding: 20px;
    }

</style>