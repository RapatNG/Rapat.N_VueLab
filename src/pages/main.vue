<template>
  <div class="container">
    <manufacturer v-slot="data">
      <devices :manufacturerId="data.factId"></devices>
    </manufacturer>
  </div>
</template>

<script>
import manufacturer from "@/components/manufacturer.vue";
import devices from "@/components/devices.vue";
export default {
  components: {
    Manufacturer: manufacturer,
    Devices: devices,
  },
};
</script>