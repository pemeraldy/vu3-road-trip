<template>
  <div class="home">
    <items-list-component :items="items" />
  </div>
</template>

<script lang="ts" >
import { defineComponent} from 'vue';
import ItemsListComponent from '@/components/items/ItemsListComponent.vue';
export default defineComponent({
  name: 'Home',
  components:{
    ItemsListComponent
  },
  setup(){
    const items: any[] =[
      {id: 1, name:'item 1'},
      {id: 2, name:'item 2'},
      {id: 3, name:'item 3'},
      {id: 4, name:'item 4'},
      {id: 5, name:'item 5'},
    ]
    return{ items}
  }
})
</script>

<style>

</style>