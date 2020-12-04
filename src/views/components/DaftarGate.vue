<template>
  <v-container>
    <v-row justify="center">
      <v-col cols="8">
        <v-card>
          <v-card-text>
            <center>
              <h1>Daftar Gate</h1>
            </center>
            <v-simple-table>
              <thead>
                <tr>
                  <th class="text-left">No</th>
                  <th class="text-left">Gate</th>
                  <th class="text-left">Status</th>
                </tr>
              </thead>
              <tbody>
                <tr v-for="item in gates" :key="item.gates">
                  <td>{{ item.nomor }}</td>
                  <td>{{ item.gates }}</td>
                  <td>{{ item.status }}</td>
                </tr>
              </tbody>
            </v-simple-table>
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "DaftarPengunjung",

  data: () => ({
    ecosystem: [
      {
        text: "vuetify-loader",
        href: "https://github.com/vuetifyjs/vuetify-loader",
      },
      {
        text: "github",
        href: "https://github.com/vuetifyjs/vuetify",
      },
      {
        text: "awesome-vuetify",
        href: "https://github.com/vuetifyjs/awesome-vuetify",
      },
    ],
    importantLinks: [
      {
        text: "Documentation",
        href: "https://vuetifyjs.com",
      },
      {
        text: "Chat",
        href: "https://community.vuetifyjs.com",
      },
      {
        text: "Made with Vuetify",
        href: "https://madewithvuejs.com/vuetify",
      },
      {
        text: "Twitter",
        href: "https://twitter.com/vuetifyjs",
      },
      {
        text: "Articles",
        href: "https://medium.com/vuetify",
      },
    ],
    whatsNext: [
      {
        text: "Explore components",
        href: "https://vuetifyjs.com/components/api-explorer",
      },
      {
        text: "Select a layout",
        href: "https://vuetifyjs.com/getting-started/pre-made-layouts",
      },
      {
        text: "Frequently Asked Questions",
        href:
          "https://vuetifyjs.com/getting-started/frequently-asked-questions",
      },
    ],
    gates: [
      {
        nomor: 1,
        gates: "Gate 1",
        status: "Buka",
      },
      {
        nomor: 2,
        gates: "Gate 2",
        status: "Buka",
      },
      {
        nomor: 3,
        gates: "Gate 3",
        status: "Buka",
      },
      {
        nomor: 4,
        gates: "Gate 4",
        status: "Tutup",
      },
      {
        nomor: 5,
        gates: "Gate 5",
        status: "Tutup",
      },
      {
        nomor: 6,
        gates: "Gate 6",
        status: "Sedang Perbaikan",
      },
      {
        nomor: 7,
        gates: "Gate 7",
        status: "Buka",
      },
      {
        nomor: 8,
        gates: "Gate 8",
        status: "Buka",
      },
      {
        nomor: 9,
        gates: "Gate 9",
        status: "Buka",
      },
      {
        nomor: 10,
        gates: "Gate 10",
        status: "Buka",
      },
    ],
  }),
};
</script>
