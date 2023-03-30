<template>
  <div class="row q-col-gutter-md">
    <div v-for="n in 18" :key="n" class="col-12 col-sm-6 col-md-4 col-lg-3">
      <q-card class="my-card">
        <q-img
          ratio="1"
          src="https://images.pexels.com/photos/128234/pexels-photo-128234.jpeg?auto=compress&cs=tinysrgb&dpr=1&w=500"
        >
          <div
            class="absolute-bottom text-subtitle2 flex flex-center full-height"
          >
            Title
          </div>
        </q-img>
      </q-card>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped></style>
