<template>
  <v-container>
    <v-layout text-center wrap>
      <v-flex xs12>
        <v-img :src="require('../assets/logo.svg')" class="my-3" contain height="200"></v-img>
      </v-flex>

      <v-flex mb-4>
        <h1 class="display-2 font-weight-bold mb-3">Welcome to Vuetify</h1>
        <p class="subheading font-weight-regular">
          For help and collaboration with other Vuetify developers,
          <br />please join our online
          <a
            href="https://community.vuetifyjs.com"
            target="_blank"
          >Discord Community</a>
        </p>
      </v-flex>

      <v-flex mb-5 xs12>
        <h2 class="headline font-weight-bold mb-3">What's next?</h2>

        <v-layout justify-center>
          <a
            v-for="(next, i) in whatsNext"
            :key="i"
            :href="next.href"
            class="subheading mx-3"
            target="_blank"
          >{{ next.text }}</a>
        </v-layout>
      </v-flex>

      <v-flex xs12 mb-5>
        <h2 class="headline font-weight-bold mb-3">Important Links</h2>

        <v-layout justify-center>
          <a
            v-for="(link, i) in importantLinks"
            :key="i"
            :href="link.href"
            class="subheading mx-3"
            target="_blank"
          >{{ link.text }}</a>
        </v-layout>
      </v-flex>

      <v-flex xs12 mb-5>
        <h2 class="headline font-weight-bold mb-3">Ecosystem</h2>

        <v-layout justify-center>
          <a
            v-for="(eco, i) in ecosystem"
            :key="i"
            :href="eco.href"
            class="subheading mx-3"
            target="_blank"
          >{{ eco.text }}</a>
        </v-layout>
      </v-flex>

      <v-row>
        <v-col cols="12">
          <p>Normal</p>
        </v-col>

        <v-col cols="12">
          <div class="text-center">
            <div class="my-2">
              <v-btn color="secondary" fab x-small dark>
                <v-icon>mdi-television</v-icon>
              </v-btn>
            </div>
            <div class="my-2">
              <v-btn color="primary" fab small dark>
                <v-icon>mdi-pencil</v-icon>
              </v-btn>
            </div>
            <div class="my-2">
              <v-btn color="warning" fab dark>
                <v-icon>mdi-account-circle</v-icon>
              </v-btn>
            </div>
            <div class="my-2">
              <v-btn color="error" fab large dark>
                <v-icon>mdi-alarm</v-icon>
              </v-btn>
            </div>
            <div class="my-2">
              <v-btn color="success" fab x-large dark>
                <v-icon>mdi-domain</v-icon>
              </v-btn>
            </div>
          </div>
        </v-col>

        <v-col cols="12" sm="3">
          <v-btn text icon color="pink">
            <v-icon>mdi-heart</v-icon>
          </v-btn>
        </v-col>

        <v-col cols="12" sm="3">
          <v-btn text icon color="indigo">
            <v-icon>mdi-star</v-icon>
          </v-btn>
        </v-col>

        <v-col cols="12" sm="3">
          <v-btn text icon color="green">
            <v-icon>mdi-cached</v-icon>
          </v-btn>
        </v-col>

        <v-col cols="12" sm="3">
          <v-btn text icon color="deep-orange">
            <v-icon>mdi-thumb-up</v-icon>
          </v-btn>
        </v-col>
      </v-row>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  name: "HelloWorld",

  data: () => ({
    ecosystem: [
      {
        text: "vuetify-loader",
        href: "https://github.com/vuetifyjs/vuetify-loader"
      },
      {
        text: "github",
        href: "https://github.com/vuetifyjs/vuetify"
      },
      {
        text: "awesome-vuetify",
        href: "https://github.com/vuetifyjs/awesome-vuetify"
      }
    ],
    importantLinks: [
      {
        text: "Documentation",
        href: "https://vuetifyjs.com"
      },
      {
        text: "Chat",
        href: "https://community.vuetifyjs.com"
      },
      {
        text: "Made with Vuetify",
        href: "https://madewithvuejs.com/vuetify"
      },
      {
        text: "Twitter",
        href: "https://twitter.com/vuetifyjs"
      },
      {
        text: "Articles",
        href: "https://medium.com/vuetify"
      }
    ],
    whatsNext: [
      {
        text: "Explore components",
        href: "https://vuetifyjs.com/components/api-explorer"
      },
      {
        text: "Select a layout",
        href: "https://vuetifyjs.com/layout/pre-defined"
      },
      {
        text: "Frequently Asked Questions",
        href: "https://vuetifyjs.com/getting-started/frequently-asked-questions"
      }
    ]
  })
};
</script>
