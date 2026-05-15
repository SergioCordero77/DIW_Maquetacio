Animacions

1. Quan pases per sobre dels elements del nav pugen 3px.
.menu-principal a{
    transition: 1s;       
}

.menu-principal a:hover {       /* Accions que es realitze quan passem el ratolí per sobre de l'element */
    text-decoration: underline; /* Apareix subrallat */           
    transform: translateY(-3px);
    transition: 1s;
}

2. Quan pases pel botó fix de reservar es fa més gran
.reservar-btn{
    transition: 1s;
}

.reservar-btn:hover {      /* Quan passem el ratolí per sobre */
    transform: scale(1.2);
    transition: 1s;
}

3. Quan pases per l'informació de contacte, les icones roten 360º
.contact-botons i {
    transition: 1s;
}

.contact-botons:hover i {
    transform: rotateY(360deg);
    transition: 1s;
}


Animació en 4 frames del botó fix de reservar

@keyframes boto {
    0% {
        transform: translateX(-300%) scale(0.25);
        background-color: white;
        opacity: 0;
    }
    33% {
        transform: translateX(-200%) scale(0.5);
        background-color: #91c3f8;
        opacity: 40%;
    }
    66% {
        transform: translateX(-100%) scale(0.75);
        background-color: #449af7;
        opacity: 80%;
    }
    100% {
        transform: translateX(0);
        background-color: var(--color-principal);
        padding: 0.5rem 1.1rem;
    }
}
