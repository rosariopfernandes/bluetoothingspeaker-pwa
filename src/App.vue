<template>
  <div class="page-container md-layout-column">
    <md-toolbar class="md-primary">
      <md-button class="md-icon-button" @click="showNavigation = true">
        <md-icon>menu</md-icon>
      </md-button>
      <span class="md-title">bluetoothingspeaker</span>
    </md-toolbar>

    <md-drawer :md-active.sync="showNavigation" md-swipeable>
      <md-toolbar class="md-transparent" md-elevation="0">
        <span class="md-title">bluetoothingspeaker</span>
      </md-toolbar>

      <md-list>
        <md-list-item>
          <md-icon>speaker</md-icon>
          <router-link :to="{ name: 'MyDevice'}" class="md-list-item-text">My Device</router-link>
        </md-list-item>

        <md-list-item>
          <md-icon>settings</md-icon>
          <span class="md-list-item-text">Settings</span>
        </md-list-item>

        <md-list-item>
          <md-icon>exit_to_app</md-icon>
          <span class="md-list-item-text">Log Out</span>
        </md-list-item>
      </md-list>
    </md-drawer>

    <md-content>
      <router-view/>
    </md-content>
  </div>
</template>

<script>
  export default {
    name: 'Temporary',
    data: () => ({
      showNavigation: false,
      showSidepanel: false
    })
  }
</script>

<style scoped>
  .page-container {
    min-height: 300px;
    overflow: hidden;
    position: relative;
    /*border: 1px solid rgba(#000, .12);*/
  }


  md-drawer {
    width: 230px;
    max-width: calc(100vw - 125px);
  }

  md-content {
    padding: 16px;
  }
</style>
