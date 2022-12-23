<!-- @format -->

<template>
	<ionApp>
    <ionPage>
      <ionHeader :translucent="true">
        <ionToolbar>
          <ionTitle>Blank</ionTitle>
        </ionToolbar>
      </ionHeader>
      <ionContent :fullscreen="true">
        <ionTabs
          @ionTabsWillChange="beforeTabChange"
          @ionTabsDidChange="afterTabChange"
          ><ionRouterOutlet></ionRouterOutlet>
          <ionTabBar slot="bottom"
            ><ionTabButton tab="home" href="/tabs/home"
              ><IonIcon :icon="ioniconsHome"></IonIcon>
              <ionLabel>Home</ionLabel></ionTabButton
            ><ionTabButton tab="schedule" href="/tabs/schedule"
              ><ionLabel>Schedule</ionLabel></ionTabButton
            ></ionTabBar
          >
          <!--  -->
        </ionTabs>
      </ionContent>
    </ionPage>
  </ionApp>
</template>


<script setup lang="ts">
const beforeTabChange = () => {
	// do something before tab change
};
const afterTabChange = () => {
	// do something after tab change
};
</script>
