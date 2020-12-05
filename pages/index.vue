<template>
  <div class="index">
    <BoardList v-model="boards" />
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import BoardList from '../components/BoardList.vue';

export default Vue.extend({
  components: {
    BoardList,
  },

  data() {
    return {
      boards: [
        {
          id: '1',
          title: '部署１',
          childs: [
            { id: '1', name: 'ほげほげ' },
            { id: '2', name: 'いいいい' },
          ],
        },
        {
          id: '2',
          title: '部署2',
          childs: [
            { id: '3', name: 'うううう' },
            { id: '4', name: 'ええええ' },
          ],
        },
        {
          id: '3',
          title: '部署3',
          childs: [
            { id: '4', name: 'うううう' },
            { id: '5', name: 'ええええ' },
          ],
        },
      ],
    };
  },
});
</script>

<style lang="scss" scoped></style>
