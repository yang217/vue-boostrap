<template>
    <div>
    <h1>{{message.name}}</h1>  
    </div>
</template>

<script>
export default {
  props:['message']
}
</script>

<style lang='scss' scoped>
    $color:red;
    h1{
        background: $color;
    }
</style>
