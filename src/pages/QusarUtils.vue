<template>
  <q-page class="q-pa-xl">
    <section class="q-mb-xl">
      <div class="text-h4">Date Util</div>
      <q-separator class="q-my-md" />
      <div class="text-h6">
        formatDate - {{ formatDate(new Date(), Format) }}
      </div>
      <div class="text-h6">
        addToDate - {{ formatDate(addToDate(new Date(), { days: 7 }), Format) }}
      </div>
      <div class="text-h6">
        subtractFromDate -
        {{ formatDate(subtractFromDate(new Date(), { days: 7 }), Format) }}
      </div>
    </section>
    <section class="q-mb-xl">
      <div class="text-h4">Format Util</div>
      <q-separator class="q-my-md" />

      <div class="text-h6">pad - {{ pad('hello', 10, '?') }}</div>
    </section>
    <section class="q-mb-xl">
      <div class="text-h4">Type Checking Util</div>
      <q-separator class="q-my-md" />

      <div class="text-h6">objA === objB - {{ objA === objB }}</div>
      <div class="text-h6">
        deepEqual(objA, objB) - {{ deepEqual(objA, objB) }}
      </div>
    </section>
  </q-page>
</template>

<script setup>
import { date, format, is } from 'quasar';

const { formatDate, addToDate, subtractFromDate } = date;
const Format = 'YYYY-MM-DD';
const { pad } = format;

const objA = { name: 'bbc' };
const objB = { name: 'bbc' };
const { deepEqual } = is;
</script>

<style lang="scss" scoped></style>
