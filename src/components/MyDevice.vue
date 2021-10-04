<template>
  <div class="md-layout md-gutter md-alignment-center">
    <md-card class="md-card md-layout-item md-medium-size-33 md-small-size-50 md-xsmall-size-100 md-large-size-50" style="padding-left: 0; padding-right: 0">
      <md-card-area>
        <md-card-media>
          <!--<img :src="cause.causeImage">-->
        </md-card-media>

        <md-card-header>
          <div class="md-title">Title</div>
          <div class="md-subhead">
            <!--Organizado por {{ cause.organizationName }}-->
          </div>
        </md-card-header>
        <md-card-content>
          <div>
            <md-button class="md-raised md-accent">Pair</md-button>
            <md-button class="md-raised md-accent">Disconnect</md-button>
          </div>
          <div>
            <md-button class="md-icon-button md-accent">
              <md-icon>volume_down</md-icon>
            </md-button>
            <span style="max-height: 40px; margin:0 auto">Volume 50/100</span>
            <md-button class="md-icon-button md-accent">
              <md-icon>volume_up</md-icon>
            </md-button>
          </div>
        </md-card-content>
      </md-card-area>
    </md-card>

    <!--<md-card class="md-card md-layout-item md-medium-size-33 md-small-size-50 md-xsmall-size-100 md-large-size-50" >-->
      <!--<md-card-content>-->
        <!--&lt;!&ndash;{{ // cause.causeDescription }}&ndash;&gt;-->
      <!--</md-card-content>-->
    <!--</md-card>-->

    <!--<md-card class="md-card md-layout-item md-medium-size-33 md-small-size-50 md-xsmall-size-100 md-large-size-50" >-->
      <!--<md-card-content>-->
        <!--Doar com M-Pesa-->
        <!--<form @submit="false">-->
          <!--<md-field>-->
            <!--<label>Valor a doar</label>-->
            <!--<span class="md-prefix">MZN</span>-->
            <!--<md-input type="number" v-model="amount"></md-input>-->
          <!--</md-field>-->
          <!--<md-field>-->
            <!--<label>Número de celular</label>-->
            <!--<md-input type="number" v-model="senderPhoneNumber"></md-input>-->
          <!--</md-field>-->
          <!--&lt;!&ndash;<md-button @click="donate(amount, senderPhoneNumber, cause.id)" class="md-raised md-accent" style="align-self: center" type="button">Doar</md-button>&ndash;&gt;-->
        <!--</form>-->
      <!--</md-card-content>-->
    <!--</md-card>-->

  </div>
</template>

<script>
export default {
  name: 'MyDevice',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .md-card {
    margin: 8px;
    display: inline-block;
    vertical-align: top;
  }
  md-button {
    min-width: 60px;
    border-radius: 2px;
  }
</style>
