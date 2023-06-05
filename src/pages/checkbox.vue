<template>
  <section>
    <div class="field">
      <o-checkbox disabled 
      checkClass="w-4 h-4"
      labelClass="ml-2 text-sm font-medium text-gray-400 dark:text-gray-500">Disabled</o-checkbox>
    </div>
    <div class="field">
      <o-checkbox :value="true" 
      checkClass="w-4 h-4"
      labelClass="ml-2 text-sm font-medium text-gray-900 dark:text-gray-300"> Default
      </o-checkbox>
    </div>    
    <div class="field">
      <o-checkbox :value="true" variant="danger"
        checkClass="w-4 h-4"
        labelClass="ml-2 text-sm font-medium text-gray-900 dark:text-gray-300"> Red </o-checkbox>
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
  @apply  text-blue-600 border-gray-300 rounded focus:ring-blue-500 dark:focus:ring-blue-600 dark:ring-offset-gray-800 focus:ring-2 dark:bg-gray-700 dark:border-gray-600
}
.o-chk--danger input{
  @apply text-red-600 bg-gray-100 border-gray-300 rounded focus:ring-red-500 dark:focus:ring-red-600 dark:ring-offset-gray-800 focus:ring-2 dark:bg-gray-700 dark:border-gray-600
}
</style>
    