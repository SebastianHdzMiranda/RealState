# aspect-ratio

# transparentize

# bucles

     Bucles en SASS
        la sintaxis es la siguiente.

        - indica una variable '$i como iterador, 
        - indica un intervalo que quieres que se ejecute tu codigo, en este ejemplo del 1 hasta el 6 'from 1 through 6'

    @for $i from 1 through 6 {
        // variable
        $imagen: '../img/propiedad_' + $i + '.jpg';
        
        // sintaxis param -> #{nombreIterador}
        &:nth-child(#{$i}) &__header {
            background-image: url($imagen);
        }
    }

# Condicionales
    se puede condicionar una propiedad en los mixins atraves de sus parametros, Ej:

        //desde el mixin
        @mixin heading($bgNegro: false) {
            
            color: #fff;

            @if($bgNegro){
                color: #000;
            }

        }

        // desde la declaracion
        @include m.heading(true);
        @include m.heading; //no se aplica la condicion

    


    