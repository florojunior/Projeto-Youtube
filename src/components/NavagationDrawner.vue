<template>
  <v-card
  style=" height:1220px;"
  >
    <v-app-bar

        style="padding:10px; height:69px"
        color="#FFFFFF"
        prominent
    >
      <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
      <div class="img">
        <v-img src="@/assets/img/youtube-logo.png"> </v-img>
      </div>
      <div class="input-search">
        <div class="input-col-all">
           <v-col
            class="col-input"
            >
            <v-text-field
                label="Pesquisar"
                append-icon="mdi mdi-keyboard"
                solo
                clearable
            ></v-text-field>
            <v-btn class="btn-form"  color="gray">  <v-icon>mdi mdi-magnify</v-icon></v-btn>
             <v-btn class="btn-form-voice " >   <v-icon>mdi mdi-microphone</v-icon></v-btn>
           
            </v-col>
        </div>
    <div class="input-icon-btn">
        <v-btn icon>
            <v-icon>mdi-bell</v-icon>
        </v-btn>

        <v-btn icon>
            <v-icon>mdi-video</v-icon>
        </v-btn>

        <v-btn icon>
            <v-icon>mdi-apps</v-icon>
        </v-btn>
        <div class="icon-user">
          <v-list-item-avatar>
              <v-img src="https://randomuser.me/api/portraits/women/85.jpg"></v-img>
            </v-list-item-avatar>
            </div>
    </div>

    </div>

        </v-app-bar>
       
    <v-navigation-drawer
    style="height:1220px; padding: 22px 36px;"
      v-model="drawer"
      absolute
      temporary
    > 
    <div class="logo-drawner">
    <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
     <div class="img-left">
        <v-img src="@/assets/img/youtube-logo.png"> </v-img>
      </div>
    </div>
      <v-list 
      class="list-tem"
      style="padding:0px"
        nav
        dense
      >
        <v-list-item-group
          v-model="group"
          active-class="deep-purple--text text--accent-4"
        >
          <v-list-item>
            <v-list-item-title> <v-icon class="icon-list">mdi mdi-home-outline </v-icon>Home</v-list-item-title>
          </v-list-item>
          <v-list-item>
             <v-list-item-title> <v-icon class="icon-list">mdi mdi-compass-outline </v-icon>Explorar</v-list-item-title>
          </v-list-item>
          <v-list-item>
             <v-list-item-title> <v-icon class="icon-list">mdi mdi-cards-playing-outline </v-icon>Shorts</v-list-item-title>
          </v-list-item>
          <v-list-item>
              <v-list-item-title> <v-icon class="icon-list">mdi mdi-account-outline</v-icon>Inscrições</v-list-item-title>
          </v-list-item>
          <hr>
          <v-list-item>
            <v-list-item-title> <v-icon class="icon-list">mdi mdi-library-outline</v-icon>Biblioteca</v-list-item-title>
          </v-list-item>
          <v-list-item>
             <v-list-item-title> <v-icon class="icon-list">mdi mdi-restore </v-icon>Historico</v-list-item-title>
          </v-list-item>
          <v-list-item>
             <v-list-item-title> <v-icon class="icon-list">mdi mdi-play-box-outline </v-icon>Seus Videos</v-list-item-title>
          </v-list-item>
          <v-list-item>
              <v-list-item-title> <v-icon class="icon-list">mdi mdi-av-timer</v-icon>Assistir mais tarde</v-list-item-title>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
    <div class="display-video-all">
        <div class="display-video">
            <iframe width="90%" height="90%" src="https://www.youtube.com/embed/yzTuBuRdAyA" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
        </div>
        <div class="display-video-right">
            <div> 
                <v-btn class="btn-small" small rounded color="gray">Todos</v-btn>
                <v-btn class="btn-small" small rounded color="gray" >Assistidos</v-btn>
                <v-btn class="btn-small"  small rounded color="gray" >Relacionados</v-btn>
           </div>
            <div class="video-right-text">
                <iframe width="270" height="150" src="https://www.youtube.com/embed/yzTuBuRdAyA" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                 <div class="video-text">
                    <h1 style="font-weight: bold; font-size:15px">Depeche Mode - Enjoy The Silence (Official Video)</h1>
                    <p>TOTO <v-icon>mdi mdi-music-note </v-icon></p>
                </div>
            </div>
            <div class="video-right-text">
                <iframe width="270" height="150" src="https://www.youtube.com/embed/yzTuBuRdAyA" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                 <div class="video-text">
                   <h1 style="font-weight: bold; font-size:15px">Depeche Mode - Enjoy The Silence (Official Video)</h1>
                    <p>TOTO <v-icon>mdi mdi-music-note </v-icon></p>
                </div>
            </div>
            <div class="video-right-text">
                <iframe width="270" height="150" src="https://www.youtube.com/embed/yzTuBuRdAyA" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                 <div class="video-text">
                    <h1 style="font-weight: bold; font-size:15px">Depeche Mode - Enjoy The Silence (Official Video)</h1>
                    <p>TOTO <v-icon>mdi mdi-music-note </v-icon></p>
                </div>
            </div>
            <div class="video-right-text">
                <iframe width="270" height="150" src="https://www.youtube.com/embed/yzTuBuRdAyA" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                 <div class="video-text">
                    <h1 style="font-weight: bold; font-size:15px">Depeche Mode - Enjoy The Silence (Official Video)</h1>
                    <p>TOTO <v-icon>mdi mdi-music-note </v-icon></p>
                </div>
            </div>
            <div class="video-right-text">
                <iframe width="270" height="150" src="https://www.youtube.com/embed/yzTuBuRdAyA" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                 <div class="video-text">
                    <h1 style="font-weight: bold; font-size:15px">Depeche Mode - Enjoy The Silence (Official Video)</h1>
                    <p>TOTO <v-icon>mdi mdi-music-note </v-icon></p>
                </div>
            </div>
        </div>
    </div>
    <v-card-text>
      outros btns que vao entrar 
    </v-card-text>
  </v-card>
  
</template>

<script>
  export default {
    name:'NagationDrawner',
    data: () => ({
      drawer: false,
      group: null,
    }),

    watch: {
      group () {
        this.drawer = false
      },
    },
  }
</script>

<style>
.search {
    padding: 0px;
}
.img {
    justify-content: center;
    align-items: center;
    margin-top: 12px;
    margin-right: 10px;
    width: 98px;
}

.display-video-all {
    display: flex;
    flex-direction: row;
    margin-top: 20px;
    justify-content: center;
    margin-left: 20px;
    padding: 20px;
}
.display-video {
    display: flex;
    flex: 100%;
    max-height: 801px;
    justify-content: end;
}
.display-video-right {
    display: flex;
    flex-direction: column;
    flex: 32%;
    align-items: flex-start;
    margin-left: 20px;
}
.video-right-text {
    display: flex;
    flex-direction: row;
    margin-bottom: 10px;
}
.video-text {
    margin-left: 13px;
    margin-top: 5px;
}
.btn-small {
    margin-right: 10px;
    margin-bottom: 10px;
}
.v-btn:focus {
    color: #303030 !important;;
}
.img-left {
    width: 40%;
    margin-top: 0px;
    margin-right: 0px;
    margin-left: 20px;
}
.logo-drawner {
    display: flex;
    align-items: center;
}
.icon-list {
    margin-right: 22px;
}
.input-search {
    display: flex;
    width: 100%;
    flex-direction: row;
    justify-content: space-around;
}
.col-input {
    display: flex;
    width: 100%;
        padding-top: 0px !important;
    padding-right: 0px !important;
    padding-bottom: 0px !important;
    padding-left: 0px !important;
}
.input-col-all {
    display: flex;
    width: 50%;
}
.icon-user {
    display: flex;
    width: 100%;
    justify-content: end;
}
.input-icon-btn {
    display: flex;
    justify-content: space-evenly;
    width: 20%;
    align-items: flex-start;
}
.btn-form {
    background: rgb(244, 244, 244) !important;

    height: 48px !important;
}
.btn-form-voice {
    background: white !important;
    border-style: none !important;
    box-shadow: none !important;
    height: 48px !important;
    outline: none !important;
    border-radius: 50px !important;
        margin-left: 10px;
}

</style>