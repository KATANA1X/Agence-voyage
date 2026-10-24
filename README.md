KATANA VOYAGE - Page d'atterrissage d'une agence de voyage

Page d'atterrissage responsive d'une agence de voyage fictive, spécialisée dans la découverte de la Côte d'Ivoire. Projet réalisé avec les composants Bootstrap.

Technologies
HTML5 et CSS3
Bootstrap 5.3.3 (grille, navbar, cards, badges, accordéon, formulaires)
Font Awesome 6.5.1 (icônes des réseaux sociaux)
Structure de la page
Barre de navigation : logo et nom de l'agence à gauche, liens (Accueil, Destinations, Circuits, Contact) à droite, menu hamburger sur mobile
Section héros : image de fond, titre, sous-titre et bouton d'appel à l'action centrés
Destinations : trois cards (Yamoussoukro, Abidjan, Bouaké), chacune avec une image, un badge de catégorie et une brève description
Circuits : accordéon Bootstrap, chaque circuit avec un titre, une description et un lien "Voir les détails"
Contact : formulaire Bootstrap (nom, adresse e-mail, destination d'intérêt, message)
Pied de page : icônes de réseaux sociaux et mention des droits d'auteur
Choix de conception
Mobile First : les colonnes s'empilent par défaut (col-12), puis passent à trois colonnes à partir de 768px (col-md-4).
Héros lisible : un voile sombre semi-transparent est posé sur la photo de fond, pour que le texte blanc reste lisible.
Images homogènes : les images des cards ont une hauteur fixe et sont recadrées sans déformation (object-fit: cover).
Couleurs : barre de navigation et pied de page sombres, bouton d'appel à l'action jaune, repris des couleurs du logo.
Badges : une couleur différente par catégorie (culture, ville, nature) pour distinguer les destinations.
Accessibilité : texte alt sur chaque image, label relié à chaque champ du formulaire, aria-label sur les liens qui ne contiennent qu'une icône, lang="fr".
Problèmes rencontrés et solutions
Classes inconnues de Bootstrap. Les éléments de la navbar portaient des classes nav-item1 à nav-item4, que Bootstrap ne reconnaît pas. Solution : utiliser exactement la classe nav-item.
Contenu incohérent après un changement de thème. Après avoir remplacé les destinations japonaises par des destinations ivoiriennes, la photo du héros, les circuits et les options du formulaire racontaient encore le Japon. Solution : tout aligner sur le même thème, jusqu'aux options du formulaire.
Images de tailles différentes dans les cards. Les photos n'avaient pas les mêmes proportions, donc les cards n'étaient pas alignées. Solution : une hauteur fixe avec object-fit: cover.
Tests

La page a été testée avec le mode responsive de Chrome à trois tailles : environ 375px (mobile), environ 800px (tablette) et grand écran (ordinateur). On vérifie le nombre de colonnes, l'absence de débordement, le menu hamburger et le bon fonctionnement de l'accordéon.

Captures d'écran:

Version ordinateur : screenshots\version-ordinateur.png

Version mobile : screenshots\version-mobile.png


Crédits:

Photo du héros : Telecharger depuis Pinterest
Photos des destinations : Telecharger depuis pinterest
Logo : réalisé pour ce projet avec l'aide d'un assistant IA
Bibliothèques : Bootstrap et Font Awesome
Organisation des fichiers:

images/
screenshots/
index.html
README.md
styles.css
