<template>
  <section>
    <!-- <div class="field">
      <o-checkbox 
      rootClass="flex items-center mb-4"
        checkCheckedClass="w-4 h-4 text-blue-600 bg-gray-100 border-gray-300 rounded focus:ring-blue-500 dark:focus:ring-blue-600 dark:ring-offset-gray-800 focus:ring-2 dark:bg-gray-700 dark:border-gray-600"
        labelClass="ml-2 text-sm font-medium text-gray-900 dark:text-gray-300">Basic</o-checkbox>
    </div>

    <div class="field">
      <o-checkbox :indeterminate="true"> Indeterminate </o-checkbox>
    </div>

    <div class="field">
      <o-checkbox v-model="checkboxCustom" true-value="Yes" false-value="No" rootClass="flex items-center mb-4"
        checkedClass="w-4 h-4 text-blue-600 bg-gray-100 border-gray-300 rounded focus:ring-blue-500 dark:focus:ring-blue-600 dark:ring-offset-gray-800 focus:ring-2 dark:bg-gray-700 dark:border-gray-600"
        labelClass="ml-2 text-sm font-medium text-gray-900 dark:text-gray-300">
        {{ checkboxCustom }}
      </o-checkbox>
    </div>
    <div class="field">
      <o-checkbox disabled labelClass="ml-2 text-sm font-medium text-gray-400 dark:text-gray-500">Disabled</o-checkbox>
    </div>

    <o-checkbox :value="true" variant="danger"
      variantClass	="w-4 h-4 text-red-600 bg-gray-100 border-gray-300 rounded focus:ring-red-500 dark:focus:ring-red-600 dark:ring-offset-gray-800 focus:ring-2 dark:bg-gray-700 dark:border-gray-600"
      checkClass=""> Danger </o-checkbox> -->

  </section>

  <section>
    <div class="field">
      <o-checkbox disabled labelClass="ml-2 text-sm font-medium text-gray-400 dark:text-gray-500">Disabled</o-checkbox>
    </div>
    <div class="field">
      <o-checkbox :value="true" variant="danger"
        checkClass="w-4 h-4 text-blue-600 bg-gray-100 border-gray-300 rounded focus:ring-blue-500 dark:focus:ring-blue-600 dark:ring-offset-gray-800 focus:ring-2 dark:bg-gray-700 dark:border-gray-600"
        labelClass="ml-2 text-sm font-medium text-gray-400 dark:text-gray-500"> Disabled </o-checkbox>
    </div>
    <div class="field">
      <o-checkbox :value="true" labelClass="ml-2 text-sm font-medium text-gray-900 dark:text-gray-300"> Default
      </o-checkbox>
    </div>
    <div class="field">
      <o-checkbox :value="true" variant="danger"
        checkClass="w-4 h-4 text-red-600 bg-gray-100 border-gray-300 rounded focus:ring-red-500 dark:focus:ring-red-600 dark:ring-offset-gray-800 focus:ring-2 dark:bg-gray-700 dark:border-gray-600"
        labelClass="ml-2 text-sm font-medium text-gray-900 dark:text-gray-300"> Red </o-checkbox>
    </div>

    <div class="flex items-center mr-4">
      <input checked id="red-checkbox" type="checkbox" value=""
        class="w-4 h-4 text-red-600 bg-gray-100 border-gray-300 rounded focus:ring-red-500 dark:focus:ring-red-600 dark:ring-offset-gray-800 focus:ring-2 dark:bg-gray-700 dark:border-gray-600">
      <label for="red-checkbox" class="ml-2 text-sm font-medium text-gray-900 dark:text-gray-300">Red</label>
    </div>
    <div class="flex items-center mr-4">
      <input checked id="green-checkbox" type="checkbox" value=""
        class="w-4 h-4 text-green-600 bg-gray-100 border-gray-300 rounded focus:ring-green-500 dark:focus:ring-green-600 dark:ring-offset-gray-800 focus:ring-2 dark:bg-gray-700 dark:border-gray-600">
      <label for="green-checkbox" class="ml-2 text-sm font-medium text-gray-900 dark:text-gray-300">Green</label>
    </div>
  </section>
</template>
<script>
import { defineComponent, ref } from 'vue';

export default defineComponent({
  setup() {
    const checkbox = ref(false);
    const checkboxCustom = ref('Yes');

    return {
      checkbox,
      checkboxCustom,
    };
  },
});
</script>
<style>
.o-chk--disabled {
  @apply bg-gray-100 border-gray-300
}
</style>
    