<template>
  <div class="test">
    <Button type="primary" size="large">warning</Button>
    <Button type="success" size="large">Success</Button>
    <Button type="error" size="large">Error</Button>
  </div>
</template>

<script>
import Vue from 'vue';
import { Button } from 'iview';
Vue.component('Button', Button);
export default {

}
</script>
