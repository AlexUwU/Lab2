# Lab2  
<template>
    <div class="home">
        <h1>{{ msg }}</h1>
        <label for="">Numero 1:</label>
        <input type="text" id="txtN1">
        <br><br>
        <label for="">Numero 2:</label>
        <input type="text" id="txtN2">
        <br><br>
        <label for="">Respuesta:</label>
        <input type="text" id="res" >
        <br><br>
        <a v-on:click="suma" href="" class="boton_1"> SUMA </a> <br><br>
        <a v-on:click="resta" href="" class="boton_2"> RESTA </a> <br><br>
        <a v-on:click="mult" href="" class="boton_3"> MULTIPLICACION </a> <br><br>
        <a v-on:click="div" href="" class="boton_4"> DIVISION </a>


    </div>
</template>

<script>
    export default {
       name: 'home.vue',
        methods: {
           
            suma: function () {
                
                var n1 = Number(document.getElementById('txtN1').value);
                var n2 = Number(document.getElementById('txtN2').value);
                var res = n1 + n2;
               
                alert("El resultado de la operacion es: " + res);
                document.getElementById('res').value = res;
                
            },
            resta: function () {
                
                var n1 = Number(document.getElementById('txtN1').value);
                var n2 = Number(document.getElementById('txtN2').value);
                var res = n1 - n2;
                alert("El resultado de la operacion es: " + res);
                document.getElementById('res').value = res;

 
            
            }, 
            
            mult: function () {
                
                var n1 = Number(document.getElementById('txtN1').value);
                var n2 = Number(document.getElementById('txtN2').value);
                var res = n1 * n2;
                alert("El resultado de la operacion es: " + res);
                document.getElementById('res').value = res;
               
            },
            
            div: function () {
                
                var n1 = Number(document.getElementById('txtN1').value);
                var n2 = Number(document.getElementById('txtN2').value);
                var res = n1 / n2;
                alert("El resultado de la operacion es: " + res);
                document.getElementById('res').value = res;
            },
            
            
        }
    };
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style type="text/css">
    
    .boton_1 {
        text-decoration: none;
        padding: 3px;
        padding-left: 10px;
        padding-right: 10px;
        font-family: helvetica;
        font-weight: 300;
        font-size: 25px;
        font-style: italic;
        color: #006505;
        background-color: #82b085;
        border-radius: 15px;
        border: 3px double #006505;
       
    }

    .boton_1:hover {
        opacity: 0.6;
        text-decoration: none;
        
    }

    .boton_2 {
        text-decoration: none;
        padding: 3px;
        padding-left: 10px;
        padding-right: 10px;
        font-family: helvetica;
        font-weight: 300;
        font-size: 25px;
        font-style: italic;
        color: #b200ff;
        background-color: #ff00dc;
        border-radius: 15px;
        border: 3px double #006505;
       
    }

    .boton_2:hover {
        opacity: 0.6;
        text-decoration: none;
        
    }

    .boton_3 {
        text-decoration: none;
        padding: 3px;
        padding-left: 10px;
        padding-right: 10px;
        font-family: helvetica;
        font-weight: 300;
        font-size: 25px;
        font-style: italic;
        color: #00ffff;
        background-color: #0026ff;
        border-radius: 15px;
        border: 3px double #006505;
       
    }

    .boton_3:hover {
        opacity: 0.6;
        text-decoration: none;
        
    }

    .boton_4 {
        text-decoration: none;
        padding: 3px;
        padding-left: 10px;
        padding-right: 10px;
        font-family: helvetica;
        font-weight: 300;
        font-size: 25px;
        font-style: italic;
        color: #ff6a00;
        background-color: #ff0000;
        border-radius: 15px;
        border: 3px double #006505;
       
    }

    .boton_4:hover {
        opacity: 0.6;
        text-decoration: none;
        
    }
</style>
