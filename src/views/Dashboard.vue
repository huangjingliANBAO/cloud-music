<template>
  <div>
    <v-row>
      <v-col v-for="(item, i) in items" :key="i" cols="6">
        <v-card :color="item.color" dark>
          <div class="d-flex flex-no-wrap justify-space-between">
            <div>
              <v-card-title class="headline" v-text="item.title"></v-card-title>

              <v-card-subtitle v-text="item.artist"></v-card-subtitle>
            </div>

            <v-avatar class="ma-3" size="125" tile>
              <v-img :src="item.src"></v-img>
            </v-avatar>
          </div>
        </v-card>
      </v-col>
    </v-row>
    <v-row>
      <v-col cols="12">
        <v-card color="#385F73" dark>
          <v-card-title class="headline">Unlimited music now</v-card-title>

          <v-card-subtitle>Listen to your favorite artists and albums whenever and wherever, online and offline.</v-card-subtitle>

          <v-card-actions>
            <v-btn text>Listen Now</v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
    <v-row>
      <v-col cols="12">
        <v-card color="#385F73" dark>
          <v-card-title class="headline">Unlimited music now</v-card-title>

          <v-card-subtitle>Listen to your favorite artists and albums whenever and wherever, online and offline.</v-card-subtitle>

          <v-card-actions>
            <v-btn text>Listen Now</v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
    <v-row>
      <v-col cols="4">
        <v-card class="mx-auto" max-width="400">
          <v-img
            height="200px"
            src="https://cdn.vuetifyjs.com/images/cards/docks.jpg"
            class="white"
          >
            <v-card-title>Top Three</v-card-title>
          </v-img>

          <v-card-subtitle class="pb-0">Number 1</v-card-subtitle>

          <v-card-text class="text--primary">
            <div>Whitehaven Beach</div>
          </v-card-text>

          <v-card-actions>
            <v-btn class="orange" text>Share</v-btn>

            <v-btn class="orange" text>Explore</v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
      <v-col cols="4">
        <v-card class="mx-auto" max-width="400">
          <v-img
            height="200px"
            src="https://cdn.vuetifyjs.com/images/cards/docks.jpg"
            class="white"
          >
            <v-card-title>Top Three</v-card-title>
          </v-img>

          <v-card-subtitle class="pb-0">Number 2</v-card-subtitle>

          <v-card-text class="text--primary">
            <div>Whitehaven Beach</div>
          </v-card-text>

          <v-card-actions>
            <v-btn class="orange" text>Share</v-btn>

            <v-btn class="orange" text>Explore</v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
      <v-col cols="4">
        <v-card class="mx-auto" max-width="400">
          <v-img
            height="200px"
            src="https://cdn.vuetifyjs.com/images/cards/docks.jpg"
            class="white"
          >
            <v-card-title>Top Three</v-card-title>
          </v-img>

          <v-card-subtitle class="pb-0">Number 2</v-card-subtitle>

          <v-card-text class="text--primary">
            <div>Whitehaven Beach</div>
          </v-card-text>

          <v-card-actions>
            <v-btn class="orange" text>Share</v-btn>

            <v-btn class="orange" text>Explore</v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
    <v-row>
      <v-col cols="6">
        <v-card class="mt-4 mx-auto" max-width="400">
          <v-sheet class="cyan" elevation="12" max-width="calc(100% - 32px)">
            <v-sparkline :labels="labels" :value="value" class="white" line-width="2" padding="16"></v-sparkline>
          </v-sheet>

          <v-card-text class="pt-0">
            <div class="title font-weight-light mb-2">User Registrations</div>
            <v-divider class="my-2"></v-divider>
            <v-icon class="mr-2" small>mdi-clock</v-icon>
            <span class="caption font-weight-light">last registration 26 minutes ago</span>
          </v-card-text>
        </v-card>
      </v-col>
      <v-col cols="6">
        <v-card class="mt-4 mx-auto" max-width="400">
          <v-sheet class="cyan" elevation="12" max-width="calc(100% - 32px)">
            <v-sparkline :labels="labels" :value="value" class="white" line-width="2" padding="16"></v-sparkline>
          </v-sheet>

          <v-card-text class="pt-0">
            <div class="title font-weight-light mb-2">User Registrations</div>
            <v-divider class="my-2"></v-divider>
            <v-icon class="mr-2" small>mdi-clock</v-icon>
            <span class="caption font-weight-light">last registration 26 minutes ago</span>
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  name: 'Dashboard',
  data: () => ({
    labels: ['12am', '3am', '6am', '9am', '12pm', '3pm', '6pm', '9pm'],
    value: [200, 675, 410, 390, 310, 460, 250, 240],
    show: false,
    items: [
      {
        color: '#1F7087',
        src: 'https://cdn.vuetifyjs.com/images/cards/foster.jpg',
        title: 'Supermodel',
        artist: 'Foster the People'
      },
      {
        color: '#952175',
        src: 'https://cdn.vuetifyjs.com/images/cards/halcyon.png',
        title: 'Halcyon Days',
        artist: 'Ellie Goulding'
      }
    ]
  })
}
</script>

<style scoped lang="scss">
.v-sheet--offset {
  top: -24px;
  position: relative;
}
.cyan {
  background-color: #00bcd4;
  margin: 0 auto;
  position: relative;
  top: -10px;
}
.white {
  color: #ffffff;
}
.gray-text {
  color: #bdbdbd;
}
.orange {
  color: #ff9100;
}
</style>
