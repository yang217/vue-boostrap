<template>

    <div class="row">
            <b-breadcrumb :items="items" />
    <template v-for="variant in ['primary','secondary','success','outline-success','warning','danger','link']">
        <div class="col-md-4 pb-2" v-for="size in ['sm','','lg']" :key="`${variant}_${size}`">
            <b-button :size="size" :variant="variant">
                {{variant}} {{size}}
            </b-button>
        </div>
    </template>
    <template v-for="variant in ['primary','secondary','success','outline-success','warning','danger','link']">
        <div class="col-md-4 pb-2" v-for="size in ['sm','','lg']" :key="`${variant}_${size}`">
            <b-button :size="size" :variant="variant">
                {{variant}} {{size}}
            </b-button>
        </div>
    </template>
</div>
</template>


<script>
export default {
data () {
    return {
      items: [{
        text: 'Admin',
        href: '#',
        active: true
      }, {
        text: 'Manage',
        href: '#',
        disabled:true,
      
      }, {
        text: 'Library',
        
      }]
    }
  }
}
</script>

<style>

</style>
