<template>
  <q-page padding>
    <section class="row q-col-gutter-x-xl q-py-lg">
      <div class="col-12 col-sm-auto q-py-md flex">
        <!-- flex-center 안씀 -->
        <q-avatar size="150px">
          <q-img src="/hicat.png" />
        </q-avatar>
      </div>
      <div class="col-12 col-sm-grow column justify-between">
        <div class="row items-center">
          <span class="text-h6 text-weight-bold">risa.cat</span>
          <q-space />
          <div class="q-gutter-x-sm">
            <q-btn outline color="secondary" label="프로필" />
            <q-btn outline color="secondary" label="프로필" />
            <q-btn outline color="secondary" label="프로필" />
            <q-btn flat color="secondary" icon="more_horiz" />
          </div>
        </div>
        <div class="q-gutter-x-lg">
          <span>게시물 0</span>
          <span>팔로워 0</span>
          <span>팔로우 0</span>
        </div>
        <div>
          <div class="">코린이</div>
          <div class="">#ENTP</div>
          <div class="">bouldering</div>
        </div>
      </div>
    </section>
    <section>
      <div class="row no-wrap scroll q-col-gutter-x-xl">
        <div class="col-auto" v-for="n in 15" :key="n">
          <article>
            <q-avatar size="77px">
              <q-img src="/nature.png" />
            </q-avatar>
            <div class="text-center q-mt-sm">day {{ n }}</div>
          </article>
        </div>
      </div>
    </section>
    <section class="q-mt-xl">
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
    </section>
  </q-page>
</template>

<script setup></script>

<style lang="scss" scoped>
.q-page {
  background-color: #fafafa;
}
</style>
