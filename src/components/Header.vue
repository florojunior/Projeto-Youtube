<template>
 <contain>
   <div cclass="container-all">
      <div class="container" >
        <v-img class="img" src="@/img/youtube-logo.png"></v-img>
      </div>
        <div class="search-all"> 
          <div class="search">
              <v-row>
                <v-col  
                    cols="1"
                    sm="8"
                    md="12"
                  >
                    <v-text-field
                    append-icon="mdi mdi-keyboard"
                      label="Pesquisar"
                      solo
                      dense
                    ></v-text-field>
                  </v-col>
                </v-row> 
            </div>
            <div class="btn">
             <v-btn
                >
                  <v-icon>
                    mdi mdi-magnify
                  </v-icon>
                </v-btn>
              </div>
        </div>
        <div class="btn-all">
          <v-btn
                >
                  <v-icon>
                    mdi mdi-video
                  </v-icon>
                </v-btn>
                <v-btn
                >
                  <v-icon>
                    mdi mdi-apps
                  </v-icon>
                </v-btn>
                <v-btn
                >
                  <v-icon>
                    mdi mdi-bell
                  </v-icon>
                </v-btn>
        </div>
    </div>
  </contain>
</template>



<script>

export default {
  name:'Header'

}
</script>


<style scoped>
.container-all {
    width: 100%;
    display: flex;
    flex-direction: row;
    padding: 10px;
}
.container {
    display: flex;
    flex-direction: row;
    width: 100%;
    padding: 25px;
    align-items: center;
}
.img {
      width: 150px;
}
.search-all {
      display: flex;
    flex-direction: row;
    width: 70%;
    align-items: center;
}
.search {
      margin-left: 100px;
    margin-top: 25px; 
    width: 60%;
    align-items: center;
}
.btn-all {
      display: flex;
    justify-content: space-around;
    width: 20%;
}
</style>