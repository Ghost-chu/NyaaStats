<template>
  <div class="col-md-6">
    <div class="panel panel-warning">
      <div class="panel-heading">
        <h3 class="panel-title">
          <span class="glyphicon glyphicon-time" aria-hidden="true"></span>&nbsp;
          Name History
        </h3>
      </div>
      <div class="panel-body">
        <ul class="list-group">
          <name v-for="(name, key, index) in player.data.names" :key="index" :name="name"></name>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
import Name from './Name';

export default {
  name: 'NameHistory',
  props: ['player'],
  components: {
    name: Name,
  },
};
</script>
