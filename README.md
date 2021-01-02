# Polygon Browser - Gestionnaire de polygones

![Ecran Principal](https://github.com/OpusTerra/PolygonBrowser/blob/main/PolyGestionPlusScreen.jpg?raw=true)

C'est assez trivial comme fonctionnement mais laissez-moi vous en dire un peu plus long :D .

Avec la masse de caches actuellement disponibles, la meilleure façon de choisir un ensemble de caches à transférer dans le GPS est sans aucun doute l'utilisation d'un filtre polygonal. On peut toujours se faire plusieurs filtres avec des polygones différents selon les besoins mais à la longue ça commence à faire une bonne liste et c'est pourquoi je me suis bâti une macro spécialement pour gérer les différents polygones selon les voyages et déplacements que je fait.

Mais ce qu'il y a de plus important c'est que cette macro me sert à filtrer seulement les caches mystères avec coordonnées corrigées ainsi que les autres standards. Mais quelquefois quand je prépare une sortie, je veux alors avoir toutes les caches incluant les mystères non résolues. C'est pour cela qu'il y a une option pour inclure les caches mystères non résolues qui peuvent exister dans le polygone choisi.

Autre aspect intéressant de cette macro, la filtration concernant l'attribut Hiver. Il s'agit ici d'une filtration utilisant directement les attributs présents dans les GPX depuis peu. Vous avez rien d'autre à faire que de charger vos PQ comme d'habitude. Auparavant, j'avais une autre façon (UserData) de le faire mais j'ai modifié ma macro pour me servir directement des attributs nouvellement fournis par geocaching.com. J'ai mis le cas Attribut Hiver Absent en choix additionnel pour le cas où le proprio de la cache n'aurait pas spécifié Hivernal ou non ... J'aime mieux alors garder cette cache dans ma liste au cas-où!

Autre particularité: le fait de copier la sélection dans la base Temp. Ça me sert quand je veux cumuler des résultats de filtres à partir de plusieurs bases de données.

Du coté des polygones, outre le fait que cette macro permet d'appeler directement l'outil Polygone de GSAK, elle vous permet aussi de voir dans Google Maps le pourtour de chacun de vos polygones. C'est à vous de leur donner des noms qui vous disent quelque chose quand vous sauvegardez les coordonnées. Notez que le principe de copier-coller est ici utilisé pour copier les coordonnées du polygone. À des fins conviviales, la macro vous redonnera à chaque démarrage, les choix déjà faits ainsi que la liste des vertex du polygone en vigueur.
Depuis la version 2.80, j'ai ajouté un filtre additionnel et optionnel qui évalue si le champ Perso (User Data) est vide ou non. Bien souvent on inscrit dans ce champ des informations concernant une séquence de caches à visiter. Cet filtre additionnel permettera d'exclure ou d'inclure les géocaches correspondantes au test spécifié. Perso, ça me sert pour séparer les caches qui seront transférées en POI et les autres qui seront en mode géocache dans un GPS de type XML (62S, Montana 600, etc)
 
 
 Ajout Version 3.15: En cliquant sur "Recherche Polygone", vous obtiendrez un écran de recherche pour vous aider à trouver les polygones correspondants à un point donné. Pour vous en servir, faites un click souris droit sur un point de la carte et puis cliquer ensuite sur le bouton "Search for Poly". La liste des polygones incluant ce point va ensuite s'afficher. En vous déplaçant dans la liste, les polygones vont se dessiner sur la carte. Vous n'aurez qu'à sélectionner celui qui fait votre affaire.

![Recherche de polygones](https://github.com/OpusTerra/PolygonBrowser/blob/main/PolyGestion_SearchPolygon.jpg?raw=true)

Version 3.20 (Aout 2019):

Nul besoin d'obtenir une clé Google MAP API. L'application utilise maintenant Leaflet.
