<template>
    <section>
        <p @click="popAlert">点我点我，啦啦啦德玛西亚</p>
    </section>
</template>

<script>
    export default {
        methods: {
            popAlert(){
                alert(1)
            }
        }
    }
</script>


<style>
</style>