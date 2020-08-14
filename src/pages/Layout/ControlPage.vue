<template>
    <div>
      <dashboard-content> </dashboard-content>
    </div>

</template>

<script>
import DashboardContent from "./Content.vue";

export default {
  components: {
    DashboardContent,
  },
  data() {
    return {
      sidebarBackground: "green",
      sidebarBackgroundImage: require("@/assets/img/sidebar-2.jpg")
    };
  }
};
</script>
