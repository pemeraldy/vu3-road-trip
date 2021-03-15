<template>
  <div class="home">
    <items-list-component :items="items" />
  </div>
</template>

<script lang="ts" >
import { defineComponent} from 'vue';
import ItemsListComponent from '@/components/items/ItemsListComponent.vue';
import { ItemInterface } from '@/models/items/Item.interface';

export default defineComponent({
  name: 'Home',
  components:{
    ItemsListComponent
  },
  setup(): { items: ItemInterface[]; }{
    const items: ItemInterface[] = [
      {id: 1, name:'item 1', selected:false},
      {id: 2, name:'item 2', selected:false},
      {id: 3, name:'item 3', selected:false},
      {id: 4, name:'item 4', selected:false},
      {id: 5, name:'item 5', selected:false},     
    ]
    return{items}
  }
})
</script>

<style>

</style>