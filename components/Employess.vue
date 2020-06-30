<template>
  <v-container>
    <v-row justify="center" class="">
        <v-card v-for="(item, index) in employess" :key="index" class="ma-3" width="300" tag="a"
        :href="`tel: +354 ${ formatPhoneNumber(item.phoneNumber) }`">
          <v-card-title>{{ item.name }}</v-card-title>
          <v-card-subtitle>{{ item.title }}</v-card-subtitle>
          <v-card-text>
            <v-icon color="primary" size="20" class="mr-2">mdi-phone</v-icon>
            {{ item.phoneNumber }}
          </v-card-text>
        </v-card>
      </v-row>
  </v-container>
</template>

<script>
export default {
  name: 'Employess',
  data() {
    return{
      employess: [
        {
          name: 'Andri Már Óttarsson',
          title: 'Rafvirkjameistari',
          phoneNumber: '698-5700',
        },
        {
          name: 'Jón Smári Eyþórsson',
          title: 'Vélvirki',
          phoneNumber: '867-3949',
        }
      ]
    }
  },
  methods: {
    formatPhoneNumber(number) {
      const temp = number.replace(' ','').replace('-','');
      return temp.substring(0, 3) + " " + temp.substring(3);
    },
  }
}
</script>