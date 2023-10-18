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