<template>
  <v-container>
    <v-row justify="center">
      <v-col cols="8">
        <v-card>
          <v-card-text>
            <center>
              <h1>Daftar Pengunjung</h1>
            </center>
            <v-simple-table>
              <thead>
                <tr>
                  <th class="text-left">No</th>
                  <th class="text-left">Nama Pengunjung</th>
                  <th class="text-left">Umur</th>
                  <th class="text-left">Jenis Kelamin</th>
                </tr>
              </thead>
              <tbody>
                <tr v-for="item in pengunjung" :key="item.pengunjung">
                  <td>{{ item.nomor }}</td>
                  <td>{{ item.pengunjung }}</td>
                  <td>{{ item.umur }}</td>
                  <td>{{ item.jeniskelamin }}</td>
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
    pengunjung: [
      {
        nomor: 1,
        pengunjung: "Pengunjung 1",
        umur: 17,
        jeniskelamin: "Laki-Laki",
      },
      {
        nomor: 2,
        pengunjung: "Pengunjung 2",
        umur: 17,
        jeniskelamin: "Perempuan",
      },
      {
        nomor: 3,
        pengunjung: "Pengunjung 3",
        umur: 17,
        jeniskelamin: "Laki-Laki",
      },
      {
        nomor: 4,
        pengunjung: "Pengunjung 4",
        umur: 17,
        jeniskelamin: "Perempuan",
      },
      {
        nomor: 5,
        pengunjung: "Pengunjung 5",
        umur: 17,
        jeniskelamin: "Laki-Laki",
      },
      {
        nomor: 6,
        pengunjung: "Pengunjung 6",
        umur: 17,
        jeniskelamin: "Perempuan",
      },
      {
        nomor: 7,
        pengunjung: "Pengunjung 7",
        umur: 17,
        jeniskelamin: "Laki-Laki",
      },
      {
        nomor: 8,
        pengunjung: "Pengunjung 8",
        umur: 17,
        jeniskelamin: "Perempuan",
      },
      {
        nomor: 9,
        pengunjung: "Pengunjung 9",
        umur: 17,
        jeniskelamin: "Laki-Laki",
      },
      {
        nomor: 10,
        pengunjung: "Pengunjung 10",
        umur: 17,
        jeniskelamin: "Perempuan",
      },
    ],
  }),
};
</script>
