<template>
  <div>
    <v-container>
      <v-row align="center">
        <v-col cols="5">
          <app-block-title no-page-title :data="titleData" class="pr-8" />
        </v-col>
        <v-col cols="7">
          <v-img
            src="@/assets/images/backgrounds/bg-spaceman.jpg"
            max-width="100%"
          />
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  components: {
    AppBlockTitle: () => import('@/core/components/AppBlockTitle')
  },
  data: vm => ({
    titleData: {
      textProps: '',
      toptitle: '',
      title: vm.$t('aboutUs.what-is-mew.title'),
      description: vm.$t('aboutUs.what-is-mew.description'),
      centered: false
    }
  })
};
</script>
