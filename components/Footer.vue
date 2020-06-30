<template>
  <footer>
    <v-container fluid>
      <v-row justify="center" align="center" class="my-3">

        <a href="mailto:straumkul@straumkul.is" class="mx-6 my-3 text-h6 black--text">
          <v-icon size="30" color="primary">mdi-email</v-icon>
          straumkul@straumkul.is
        </a>

        <a href="https://www.google.com/maps/place/Lyngh%C3%A1ls+3,+Reykjav%C3%ADk/@64.1208853,-21.7961986,17z/data=!3m1!4b1!4m5!3m4!1s0x48d673836610ddab:0x11c25d248ccec567!8m2!3d64.120883!4d-21.7940099"
          target="_blank" class="mx-6 my-3 text-h6 black--text">
          <v-icon size="30" color="primary">mdi-map-marker</v-icon>
          Lyngháls 3, 110 Reykjavík
        </a>

      </v-row>
    </v-container>
  </footer>
</template>

<script>
  export default {
    name: 'Footer',
  }

</script>
