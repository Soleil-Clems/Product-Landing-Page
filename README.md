# Product-Landing-Page

-Nom du Projet : FreeCodeCamp Product-Landing-Page
   Il s'agit du 4eme projet de la certification Responsive design de FreeCodeCamp

-Competences mises en avant:
  Lors de ce projet j'ai appris l'importance du display grid. Les grid agissent tous comme les flexbox. Mais contrairement aux flexbox qui n'agissent que sur un seul axe a la fois, les grid agissent a la fois sur les axes des ordonnées et des abscisses.

- Difficultés:
    1.J'ai fais face a deux difficultés de tailles lors de ce projet, les deux avaient un rapport avec la responsivité du site. Le Formulaire appliquait une marge de 54em quand je reduisais la taille de l'ecran.

    2. Les parties en dessous du formulaire se separait du formulaire avec une grande marge, mais cette marge n'avait rien a voir avec les margins ou padding, c'etait du a la hauteur de #page-wrapper
    qui est le parent qui contient toute la page

- Comment resoudre les difficultées:
    1. Pour commencer j'avais cette margin parceque le header etait en posion:fixed; avec top:0; donc j'etait obligé de mettre une margin-top: 54em; pour pouvoir voir le formulaire qui etait caché derriere le header; finalement pour resoudre le probleme, j'ai changé d'approche ent mettant un display:grid; et un grid-auto-flow: row; ca m'a automatiquement rendu le site responsif.

    2.Pour resoudre le probleme de tout ce qui venait apres le formulaire, il faut d'abord savoir, que j'avais mis le #page-wrapper a height:100vh; et vu que le grid etait present, lorsque je reduisais la taille de mon ecran, il calculait automatiquement la taille nessessaire quitte a laisser de grands espace. Pour resoudre le probleme j'ai juste retirer le height: 100vh; du #page-wrapper; car au final il ne servait a rien;

- Astuces :
    L'equivalent du "flex-direction:row;" en flexbox est "grid-auto-flow: column;" dans le cas des grid. C'est bizarre de savoir qu'en grid c'est 'column' et non 'row' mais c'est le cas.
    Celui de "flex-direction:column;" est "grid-auto-flow:row;"