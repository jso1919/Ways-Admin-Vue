<template>
  <b-nav fill tabs>
    <b-nav-item :active="activeList" :to="{name:'RidesList'}">
      All <i class="icon-options-vertical" />
    </b-nav-item>

    <b-nav-item v-if="activeEdit" :active="activeEdit" >
      Edit <i class="icon-cloud-upload" />
    </b-nav-item>
  </b-nav>
</template>

<script>
export default {
  props: {
    activeList: {
      type: Boolean
    },
    activeNew: {
      type: Boolean
    },
    activeEdit: {
      type: Boolean
    }
  },
  name: 'NavTop'
}
</script>
