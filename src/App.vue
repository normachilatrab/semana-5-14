<template>
  <div>
    <div v-if="estado">
      <nav class="navbar navbar-expand-lg sticky-top navbar-dark bg-dark">
        <a class="navbar-brand" href="# ">
          <img
            src="https://www.flaticon.com/svg/static/icons/svg/3930/3930366.svg"
            width="30 "
            height="30
    "
            class="d-inline-block align-top"
            alt=" "
            loading="lazy "
          />
          Soluciones de Software S.A.S
        </a>
        <div
          class="collapse navbar-collapse justify-content-end"
          id="navbarNav "
        >
          <ul class="navbar-nav">
            <li class="nav-item active">
              <a class="nav-link" v-on:click="ingresar" href="# "
                >Sistema <span class="sr-only">(current)</span></a
              >
            </li>
          </ul>
        </div>
      </nav>
      <div
        id="carouselExampleCaptions"
        class="carousel slide"
        data-ride="carousel"
      >
        <ol class="carousel-indicators">
          <li
            data-target="#carouselExampleCaptions"
            data-slide-to="0"
            class="active"
          ></li>
          <li
            data-target="#carouselExampleCaptions"
            data-slide-to="1"
            class=""
          ></li>
          <li
            data-target="#carouselExampleCaptions"
            data-slide-to="2"
            class=""
          ></li>
        </ol>
        <div class="carousel-inner">
          <div class="carousel-item active">
            <svg
              class="bd-placeholder-img bd-placeholder-img-lg d-block w-100"
              width="800"
              height="400"
              xmlns="http://www.w3.org/2000/svg"
              preserveAspectRatio="xMidYMid slice"
              focusable="false"
              role="img"
              aria-label="Placeholder: First slide"
            >
              <title>Placeholder</title>
              <rect width="100%" height="100%" fill="#777"></rect>
              <text x="50%" y="50%" fill="#555" dy=".3em">First slide</text>
            </svg>
            <div class="carousel-caption d-none d-md-block">
              <h5>Desarrollo de Software</h5>
              <p>
                Diseñamos estrategias de crecimiento que permitan trazar nuevas
                oportunidades para su negocio.
              </p>
            </div>
          </div>
          <div class="carousel-item">
            <svg
              class="bd-placeholder-img bd-placeholder-img-lg d-block w-100"
              width="800"
              height="400"
              xmlns="http://www.w3.org/2000/svg"
              preserveAspectRatio="xMidYMid slice"
              focusable="false"
              role="img"
              aria-label="Placeholder: Second slide"
            >
              <title>Placeholder</title>
              <rect width="100%" height="100%" fill="#666"></rect>
              <text x="50%" y="50%" fill="#444" dy=".3em">Second slide</text>
            </svg>
            <div class="carousel-caption d-none d-md-block">
              <h5>Analisís de Datos</h5>
              <p>
                Ayudamos al negocio a entender los insights que arrojan sus
                datos de cara a la mejora continua.
              </p>
            </div>
          </div>
          <div class="carousel-item">
            <svg
              class="bd-placeholder-img bd-placeholder-img-lg d-block w-100"
              width="800"
              height="400"
              xmlns="http://www.w3.org/2000/svg"
              preserveAspectRatio="xMidYMid slice"
              focusable="false"
              role="img"
              aria-label="Placeholder: Third slide"
            >
              <title>Placeholder</title>
              <rect width="100%" height="100%" fill="#555"></rect>
              <text x="50%" y="50%" fill="#333" dy=".3em">Third slide</text>
            </svg>
            <div class="carousel-caption d-none d-md-block">
              <h5>Transformación Digital</h5>
              <p>
                Impulsamos las últimas tecnologías para ayudar a las
                organizaciones a transformarse
              </p>
            </div>
          </div>
        </div>
        <a
          class="carousel-control-prev"
          href="#carouselExampleCaptions"
          role="button"
          data-slide="prev"
        >
          <span class="carousel-control-prev-icon" aria-hidden="true"></span>
          <span class="sr-only">Anterior</span>
        </a>
        <a
          class="carousel-control-next"
          href="#carouselExampleCaptions"
          role="button"
          data-slide="next"
        >
          <span class="carousel-control-next-icon" aria-hidden="true"></span>
          <span class="sr-only">Siguiente</span>
        </a>
      </div>
      <div>
        <home />
      </div>
      <footer class="page-footer bg-secondary text-white pt-4">
        <!-- Footer Text -->
        <div class="container-fluid text-center text-md-left">
          <!-- Grid row -->
          <div class="row">
            <!-- Grid column -->
            <div class="col-md-6 mt-md-0 mt-3">
              <!-- Content -->
              <h5 class="text-uppercase font-weight-bold">Por qué elegirnos</h5>
              <p>
                Somos un equipo especializado creando aplicaciones moviles ,
                para que sus productos o servicios siempre esten al alcance de
                sus clients. Apicamos metodologia de punto , para desarrollar en
                menor tiempo el software que su empresa necesita utilizando
                metodologias agiles de scrum.
              </p>
            </div>
            <!-- Grid column -->

            <hr class="clearfix w-100 d-md-none pb-3" />

            <!-- Grid column -->
            <div class="col-md-6 mb-md-0 mb-3">
              <!-- Content -->
              <h5 class="text-uppercase font-weight-bold">Nuestros clientes</h5>
              <p>
                Café sello rojo. Mil variedades. Grupo Exito. EPM.<br />
                Contamos con mas de 10 años de experiencia en el Mercado
                nacional , liderando las mejores practicas de desarrollo de
                software.
              </p>
            </div>
            <!-- Grid column -->
          </div>
          <!-- Grid row -->
        </div>
        <!-- Footer Text -->

        <!-- Copyright -->
        <div class="footer-copyright text-center py-1 bg-dark">
          Todos los derechos reservados &#174;2020 - Grupo 14 MisionTIC
        </div>
        <!-- Copyright -->
      </footer>
    </div>
    <div v-else>
      <v-app id="app">
        <v-navigation-drawer
          v-model="drawer"
          :clipped="$vuetify.breakpoint.lgAndUp"
          app
        >
          <v-list dense>
            <template>
              <v-list-item @click="home">
                <v-list-item-action>
                  <v-icon>home</v-icon>
                </v-list-item-action>
                <v-list-item-title> Inicio </v-list-item-title>
              </v-list-item>
            </template>
            <template v-if="logueado">
              <v-list-group>
                <v-list-item slot="activator">
                  <v-list-item-content>
                    <v-list-item-title> Almacén </v-list-item-title>
                  </v-list-item-content>
                </v-list-item>
                <v-list-item :to="{ name: 'categoria' }">
                  <v-list-item-action>
                    <v-icon>table_chart</v-icon>
                  </v-list-item-action>
                  <v-list-item-content>
                    <v-list-item-title> Categorías </v-list-item-title>
                  </v-list-item-content>
                </v-list-item>
                <v-list-item :to="{ name: 'articulo' }">
                  <v-list-item-action>
                    <v-icon>table_chart</v-icon>
                  </v-list-item-action>
                  <v-list-item-content>
                    <v-list-item-title> Artículos </v-list-item-title>
                  </v-list-item-content>
                </v-list-item>
              </v-list-group>
              <v-list-group>
                <v-list-item slot="activator">
                  <v-list-item-content>
                    <v-list-item-title> Accesos </v-list-item-title>
                  </v-list-item-content>
                </v-list-item>
                <v-list-item :to="{ name: 'usuario' }">
                  <v-list-item-action>
                    <v-icon>table_chart</v-icon>
                  </v-list-item-action>
                  <v-list-item-content>
                    <v-list-item-title> Usuarios </v-list-item-title>
                  </v-list-item-content>
                </v-list-item>
              </v-list-group>
            </template>
          </v-list>
        </v-navigation-drawer>

        <v-app-bar
          :clipped-left="$vuetify.breakpoint.lgAndUp"
          app
          color="silver darken-3"
          dark
        >
          <v-toolbar-title style="width: 300px" class="ml-0 pl-3">
            <v-app-bar-nav-icon
              @click.stop="drawer = !drawer"
            ></v-app-bar-nav-icon>
            <span class="hidden-sm-and-down">Sistema</span>
          </v-toolbar-title>
          <v-spacer></v-spacer>
          <v-btn @click="salir()" icon v-if="logueado">
            <v-icon>logout</v-icon> Salir
          </v-btn>
          <v-btn :to="{ name: 'login' }" icon v-else>
            <v-icon>apps</v-icon> Login
          </v-btn>
        </v-app-bar>
        <v-content>
          <v-container fluid fill-height>
            <v-slide-y-transition mode="out-in">
              <router-view />
            </v-slide-y-transition>
          </v-container>
        </v-content>
        <v-footer height="auto">
          <v-layout justify-center>
            <v-flex text-xs-center>
              <v-card flat tile color="primary" class="white--text">
                <v-card-text class="white--text pt-0">
                  Grupo 14 Soluciones de Software &copy;2020
                </v-card-text>
              </v-card>
            </v-flex>
          </v-layout>
        </v-footer>
      </v-app>
    </div>
  </div>
</template>

<script>
import home from "./components/home.vue";
export default {
  components: { home },
  name: "App",

  data() {
    return {
      drawer: false,
      estado: 1,
    };
  },

  computed: {
    logueado() {
      return this.$store.state.usuario;
    },
  },
  created() {
    this.$store.dispatch("autoLogin");
  },
  methods: {
    salir() {
      this.$store.dispatch("salir");
      this.estado = 1;
    },

    ingresar() {
      this.estado = 0;
    },

    home() {
      this.estado = 1;
    },
  },
};
</script>
