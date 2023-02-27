<template>
  <figure class="md:flex bg-slate-100 rounded-xl p-8 md:p-0 dark:bg-slate-800">
    <img
      class="w-24 h-24 md:w-48 md:my-auto md:ml-8 rounded-full mx-auto"
      src="/sarah.jpg"
      alt=""
    />
    <div class="pt-6 md:p-8 text-center md:text-left">
      <blockquote>
        <p class="text-lg font-medium">
          “Tailwind CSS is the only framework that I've seen scale on large
          teams. It’s easy to customize, adapts to any design, and the build
          size is tiny.”
        </p>
      </blockquote>
      <figcaption class="font-medium">
        <div class="text-sky-500 dark:text-sky-400">Sarah Dayan</div>
        <div class="text-slate-700 dark:text-slate-500">
          Staff Engineer, Algolia
        </div>
        <button
          class="btn btn--primary"
          @click="onDownload"
        >
          Download
        </button>
      </figcaption>
    </div>
  </figure>
</template>

<script>
import { defineComponent } from 'vue';
export default defineComponent({
  methods: {
    onDownload() {
      const link = document.createElement('a');
      link.href = '/download';
      link.click();
    },
  },
});
</script>
