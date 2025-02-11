<template>
  <div style="max-width: min-content;min-width: fit-content; display: inline-block">
    <label>Floating Vue

      <VDropdown placement="top" :modifiers="[{ name: 'offset', options: { offset: [0, 5] } }]" class="inline">
        <i class="pi pi-info-circle"></i>
        <template #popper>
          floating-vue is a library helping you add tooltips, dropdowns and other poppers into your Vue application.
        </template>
      </VDropdown>
    </label>
  </div>
  <div>
    <p-dropdown v-model="selectedRegistrationYear" :options="registrationYear" class="w-full"></p-dropdown>
  </div>

</template>

<style>
.v-popper__popper.v-popper__popper--shown{
  max-width: 320px;
}
.v-popper--theme-dropdown .v-popper__inner{
  padding: .5rem;
  background-color: #333f48 !important;
  color: #fff !important;
}

.v-popper--theme-dropdown .v-popper__arrow-inner{
  border-color:#333f48 !important
}
</style>
