<!-- @format -->

<template lang="pug">
ionPage
   ionTabs(@ionTabsWillChange="beforeTabChange" @ionTabsDidChange="afterTabChange")
      ionRouterOutlet
      ionTabBar(slot="bottom")
         ionTabButton(tab="home" href="/tabs/home")
            ionLabel Home
         ionTabButton(tab="schedule" href="/tabs/schedule")
            ionLabel Schedule
</template>

<script setup lang="ts">
const beforeTabChange = () => {
	// do something before tab change
};
const afterTabChange = () => {
	// do something after tab change
};
</script>
