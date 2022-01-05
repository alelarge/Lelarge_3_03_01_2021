# Lelarge_3_03_01_2021

sudo ./dart-sass/sass saas/style.scss style.css
sudo ./dart-sass/sass saas/style.scss style.css --watch

style.css.map permettre au navigateur la correspondante entre ligne css et une ligne scss voir les erreurs dasn le fichier source et pas dans le dossier compilé

Imbrication scss : niveau de profondeur de 2 pour la lisibilité, sinon plus plus difficile à lire

ex:
.table {
width: 100%;

    td{
        border : 1px #FFF;
    }

}

ex : pour changer de couleur btn

btn {
background:rgb(99,125,255);

    &:hover{
        background:rgb(62,81,189);
    }

}

On peut mettre une @media only screen and(max-width:1200px) dans l'imbrication. Mais il est préférable de grouper les media.

Héritage : une balise va agir comme un autre sélecteur

call to action : même apparance comme un bouton

ex:
btn {
background:rgb(99,125,255);

    &:hover{
        background:rgb(62,81,189);
    }

}

btn-danger{
@extends .btn;

    background : red;
    &hover{
        background:
    }

}
