<template>
  <div
    class="flex flex-col md:flex-row mx-auto"
    style="max-width: 900px; font-family: Nunito"
  >
    <div class="flex flex-col mx-8 my-16 md:w-1/2">
      <div class="text-gray-700">
        Fill out the form <span class="md:hidden">below</span
        ><span class="hidden md:inline-block">to the right</span> to be added to
        a group chat at the beginning of next month with other people who are
        also new to your area.<br /><br />Minimum of 8 people in a new group,
        maximum of 24. There may be multiple groups per city per month. If there
        aren't enough people to make a new group, your enrollment will roll over
        to the next month.<br /><br />Be new together 🙃.<br /><br />
      </div>
      <div class="font-bold">Next batch: September 2021</div>
      <div class="my-16 text-6xl font-bold bg-indigo-900 stripe relative">
        <h1 class="text-white py-16">I'm new to(o)</h1>
      </div>
      <div>
        <p class="text-gray-400">September 2021 batch</p>
        <p class="text-gray-400">Counts updated ~daily</p>
        <table class="my-4">
          <tr>
            <td class="w-full">San Fransisco</td>
            <td>0</td>
          </tr>
          <tr>
            <td>Washington, DC</td>
            <td>0</td>
          </tr>
          <tr>
            <td>Seattle</td>
            <td>0</td>
          </tr>
          <tr>
            <td>Chicago</td>
            <td>0</td>
          </tr>
          <tr>
            <td>Los Angeles</td>
            <td>0</td>
          </tr>
          <tr>
            <td>New York</td>
            <td>0</td>
          </tr>
          <tr>
            <td>Miami</td>
            <td>0</td>
          </tr>
          <tr>
            <td>&lt;Your city&gt;</td>
            <td>0</td>
          </tr>
        </table>
      </div>
    </div>
    <div class="flex-grow md:w-1/2">
      <iframe
        class="airtable-embed airtable-dynamic-height"
        src="https://airtable.com/embed/shr18jf7QAOoqTNhA?backgroundColor=blue"
        frameborder="0"
        onmousewheel=""
        width="100%"
        height="1145"
        style="background: transparent; border: 1px solid #ccc"
      ></iframe>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "App",
  components: {},
});
</script>

<style>
.stripe:before {
  content: "";
  background-color: rgb(49, 46, 129);
  position: absolute;
  height: 100%;
  width: 4000px;
  left: -1000px;
  z-index: -1;
}
</style>
