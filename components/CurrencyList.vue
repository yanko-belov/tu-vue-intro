<template>
  <FilterInput v-model="filter" />
  <div id="new-component">
    <div id="filter-value">
      <!-- The filter value Must go here -->
    </div>
    <!-- The clear filter button must go here -->
    <div id="has-active-filter">
      Is the filter active: No
    </div>
  </div>
  <div>
    <button
        type="button"
        class="mt-3 rounded-lg border border-red-700 px-5 py-2.5 text-center text-sm font-medium text-red-700 hover:bg-red-800 hover:text-white focus:outline-none focus:ring-4 focus:ring-red-300"
        data-testid="clear-filter"
        @click="filter = 'ETH'"
    >
      Set filter to ETH
    </button>
  </div>
  <div
    class="mt-4 grid grid-cols-1 gap-4 min-[530px]:grid-cols-2 md:mt-6 md:grid-cols-3 md:gap-6 lg:grid-cols-4 xl:grid-cols-5"
    data-testid="card-container"
  >
    <NuxtLink
      v-for="currency in currencyListFiltered"
      :key="`currency-${currency.id}`"
      :to="`currency/${currency.symbol}`"
    >
      <CurrencyCard :symbol="currency.symbol" class="h-full" />
    </NuxtLink>
  </div>
</template>

<script lang="ts" setup>
import type { ICurrency } from "~/types";

const props = withDefaults(
    defineProps<{ currencyList: ICurrency[]; isLoading?: boolean }>(),
    {
      currencyList: () => [],
      isLoading: false,
    }
);

const filter = ref("");
const isFilterActive = computed(() => {
  // the logic to check if the filter is empty must go here
  return false;
});

const currencyListFiltered = computed(() => {
  return props.currencyList;
});
const clearFilter = () => (filter.value = "");
</script>
