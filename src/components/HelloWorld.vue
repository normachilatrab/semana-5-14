<template>
    

     
</template>

<script>
import axios from 'axios';
export default {
  name: "HelloWorld",

  data() {
        return {
            datos: null,
            team: [{
                codigo: 1,
                Nombre: 'Lucas Mera',
                Descripcion: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris condimentum ac elit et accumsan.',
                Rol: 'Desarrollador backend',
                Color: 'bg-danger'
            }, {
                codigo: 2,
                Nombre: 'Cristian Sanz',
                Descripcion: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris condimentum ac elit et accumsan.',
                Rol: 'Arquictecto de software',
                Color: 'bg-dark'
            }, {
                codigo: 3,
                Nombre: 'Samara Cerezo',
                Descripcion: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris condimentum ac elit et accumsan.',
                Rol: 'Tester',
                Color: 'bg-danger'
            }, {
                codigo: 4,
                Nombre: 'Iris Mesa',
                Descripcion: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris condimentum ac elit et accumsan.',
                Rol: 'Analista',
                Color: 'bg-dark'
            }]
        };
    },
    

  
};
</script>
