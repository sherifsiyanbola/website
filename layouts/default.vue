<template>
  <v-app class="white">
    <v-toolbar
      color="white"
      class="teal--text">
      <v-toolbar-title>VN</v-toolbar-title>
      <v-divider
        class="mx-3"
        inset
        vertical
      />

      <span class="subheading hidden-sm-and-down">Vue Nigeria</span>
      <v-spacer/>
      <v-toolbar-items>
        <v-btn
          flat
          color="teal"
          nuxt="true"
          to="/">Home</v-btn>
        <v-btn
          flat
          color="teal"
          nuxt="true"
          to="/login">Login</v-btn>
        <v-btn
          flat
          color="teal"
          nuxt="true"
          to="/register">Signup</v-btn>
      </v-toolbar-items>
    </v-toolbar>

    <nuxt/>

    <v-footer
      dark
      height="auto"
    >
      <v-card
        flat
        tile
        class="teal darken-4 white--text text-xs-center"
      >
        <v-card-text>
          <v-btn
            v-for="icon in icons"
            :key="icon"
            class="mx-3 white--text"
            icon
          >
            <v-icon size="24px">{{ icon }}</v-icon>
          </v-btn>
        </v-card-text>

        <v-card-text class="white--text pt-0">
          Phasellus feugiat arcu sapien, et iaculis ipsum elementum sit amet. Mauris cursus commodo interdum. Praesent ut risus eget metus luctus accumsan id ultrices nunc. Sed at orci sed massa consectetur dignissim a sit amet dui. Duis commodo vitae velit et faucibus. Morbi vehicula lacinia malesuada. Nulla placerat augue vel ipsum ultrices, cursus iaculis dui sollicitudin. Vestibulum eu ipsum vel diam elementum tempor vel ut orci. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.
        </v-card-text>

        <v-divider/>

        <v-card-text class="white--text">
          &copy;2018 — <strong>Vue Naigeria</strong>
        </v-card-text>
      </v-card>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data: () => ({
    icons: [
      'fab fa-facebook',
      'fab fa-twitter',
      'fab fa-google-plus',
      'fab fa-linkedin',
      'fab fa-instagram'
    ]
  })
}
</script>
