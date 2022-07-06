<template>
  <v-app id="home" :style="{ background: $vuetify.theme.themes.dark.background }">
    <nav-bar />
    <v-container fluid>
      <v-row>
        <v-col cols="6">
          <v-img src="" contain max-height="500"></v-img>
        </v-col>
        <v-col cols="6">
          <h5 class="red--text text--darken-4 top">Hola soy Brandon</h5>
          <h1 class="white--text">Desarrollador Web</h1>
          <p class="grey--text">
            Texto Aqui
          </p>
          <v-btn title color="red" dark> Acerca de mi </v-btn>
        </v-col>
        <v-col cols="12" class="padd">
          <div class="first" id="about">
            <v-row>
              <v-col cols="12">
                <div class="child bgColor1">
                  <v-icon color="red" x-large class="ml-3">mdi-school</v-icon>
                  <h3 class="white--text ml-3 mt-4">Educacion</h3>
                  <p class="grey--text ml-3 mt-6">
                    Texto aqui
                  </p>
                  <v-btn color="red" dark text>
                    Leer mas
                    <v-icon right>mdi-arrow-right</v-icon>
                  </v-btn>
                </div>
                <div class="child bgColor2">
                  <v-icon color="white" x-large class="ml-3" dark>mdi-home-city</v-icon>
                  <h3 class="white--text ml-3 mt-4">Experiencia</h3>
                  <p class="grey--text ml-3 mt-6">
                    Texto aqui
                  </p>
                  <v-btn color="" dark text>
                    Leer mas
                    <v-icon right>mdi-arrow-right</v-icon>
                  </v-btn>
                </div>
                <div class="child bgColor1">
                  <v-icon color="red" x-large class="ml-3">mdi-code-braces</v-icon>
                  <h3 class="white--text ml-3 mt-4">Tecnologias</h3>
                  <p class="grey--text ml-3 mt-6">
                    Texto aqui
                  </p>
                  <v-btn color="red" dark text>
                    Leer mas
                    <v-icon right>mdi-arrow-right</v-icon>
                  </v-btn>
                </div>
              </v-col>
              <v-col cols="12" class="mt-10">
                <div class="child1">
                  <h1 class="red--text text--darken-4 mt-4 number">1</h1>
                  <h3 class="white--text mt-4">Años de Experiencia</h3>
                </div>
                <div class="child2 mRight">
                  <v-row>
                    <v-col cols="12" class="childcol">
                      <div class="child2 mButton padding bgColor1">
                        <h1 class="red--text text--darken-4">3</h1>
                        <p class="grey--text">Clientes</p>
                      </div>
                    </v-col>
                    <v-col cols="12" class="childcol">
                      <div class="child2 padding bgColor1">
                        <h1 class="red--text text--darken-4">3</h1>
                        <p class="grey--text">Proyectos</p>
                      </div>
                    </v-col>
                  </v-row>
                </div>
              </v-col>
            </v-row>
          </div>
        </v-col>
        <v-col md="3" offset-md="3" id="project">
          <h4 class="white--text">PROYECTOS</h4>
          <p class="grey--text">Texto aqui</p>
        </v-col>
        <v-col md="3" class="text-end">
          <v-btn title color="red" dark> Ver todo </v-btn>
        </v-col>
        <v-col md="3" offset-md="3">
          <v-card class="pa-2 py-12" outlined tile height="250px" color="#1E1E1E">
            <v-img src="" contain max-height=""></v-img>
          </v-card>
        </v-col>
        <v-col md="3">
          <v-card class="pa-2 py-12" outlined tile height="250px" color="#1E1E1E">
            <v-img src="" contain max-height=""></v-img>
          </v-card>
        </v-col>
        <v-col md="3" offset-md="3">
          <v-btn color="white" dark text class="ml-n4"> MexLog </v-btn><br />

          <v-btn color="red" dark text class="ml-n4">
            Leer mas
            <v-icon right>mdi-arrow-right</v-icon>
          </v-btn>
        </v-col>
        <v-col md="3">
          <v-btn color="white" dark text class="ml-n4"> SCP Maguisterio 18 </v-btn><br />
          <v-btn color="red" dark text class="ml-n4">
            Leer mas
            <v-icon right>mdi-arrow-right</v-icon>
          </v-btn>
        </v-col>    
        <v-col cols="12" class="padd topInverse">
          <div class="second">
            <div class="secondchild1" id="contact">
              <v-row>
                <v-col cols="7">
                  <h1 class="white--text">
                    Contactame por este medio.
                  </h1>
                  <p class="grey--text">
                    Texto aqui <br />
                  </p>
                </v-col>
                <v-col cols="5">
                  <v-btn title color="red" dark class="mt-16">
                    Contacto
                  </v-btn>
                </v-col>
              </v-row>
            </div>
          </div>
          <v-toolbar class="topTolbar" color="#111111" dark flat>
          </v-toolbar>
        </v-col>
      </v-row>
    </v-container>
    <Footer />
  </v-app>
</template>

<script>
import NavBar from "../components/NavBar.vue";
import Footer from "../components/Footer.vue";
export default {
  name: "Home",
  data: () => ({
   
  }),
  components: {
    NavBar,
    Footer,
  },
};
</script>
<style scoped>
.top {
  margin-top: 180px;
}

.topInverse {
  margin-top: -250px;
}

.topTolbar {
  margin-top: 100px;
  text-align: center;
}

.first {
  width: 100%;
  height: 610px;
  background: linear-gradient(to right,
      #181818,
      #181818 50%,
      #111111 50%,
      #111111 50%);
  text-align: center;
  padding: 2rem 2rem;
}

.second {
  width: 100%;
  height: 400px;
  background: #181818;
  text-align: center;
  padding: 2rem 2rem;
}

.secondchild1 {
  display: inline-block;
  background-color: #1e1e1e;
  padding: 2rem 1rem;
  vertical-align: middle;
  text-align: left;
  margin-top: 250px;
}

.child {
  display: inline-block;
  padding: 2rem 1rem;
  vertical-align: middle;
  text-align: left;
  margin-right: 8px;
}

.bgColor1 {
  background-color: #1e1e1e;
}

.bgColor2 {
  background-color: red;
}

.child1 {
  display: inline-block;
  padding: 2rem 1rem;
  vertical-align: middle;
  margin-right: 5px;
  width: 240px;
}

.child2 {
  display: inline-block;
  width: 245px;
  vertical-align: middle;
}

.mRight {
  margin-right: 8px;
}

.mButton {
  margin-bottom: 8px;
}

.padding {
  padding: 8px 0;
}

.col-12.padd {
  padding: 12px 0 !important;
}

.col-12.childcol {
  padding: 0 !important;
}

h1.number {
  font-size: 50px;
  font-weight: bold;
}
</style>