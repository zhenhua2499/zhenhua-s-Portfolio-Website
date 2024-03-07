<template>
  <v-app class="bg-grey-lighten-5">
    <SiteHeader />
    <v-main>
      <router-view />
    </v-main>
    <v-footer theme="dark" color="grey-lighten-2 mt-5">
      <v-container class="text-center w-100 justify-space-between d-flex flex-row">
        <v-row>
          <v-col>
            <div class="align-start">
              <div class="d-flex flex-row justify-start flex-column text-start">
                <p>如果您想继续与我取得联系，可以点击"<strong><a href="#与我联系"
                      class="text-blue text-decoration-none">邮件联系</a></strong>"
                  按钮</p>
              </div>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </v-footer>
    <div class="bg-grey-lighten-2 text-center d-flex flex-column">
      <v-divider></v-divider>
      <v-subheader>
        <strong>© <a href="https://github.com/onaranyusuf" class="text-red text-decoration-none">zhenhua liu</a> —
          Theme by <a href="npm run" target="_blank" class="text-red text-decoration-none">zhenhua
            liu</a> </strong> — {{ new Date().getFullYear() }}
        <v-spacer></v-spacer>
      </v-subheader>
    </div>
  </v-app>
</template>

<script>
import SiteHeader from '@/components/header.vue';

export default {
  name: 'App',
  data: () => ({

  }),

  components: {
    SiteHeader,
  },

}
</script>

