# PCBS_Agnesoros_BoubaKiki

Introduction : 

L’effet « Bouba-kiki » en psychologie est le nom donné à l’observation, chez la grande majorité des locuteurs, quelle que soit leur langue (ainsi que chez des nouveaux-nés) de l’association d’une forme angulaire, avec des « pics/épines » (« spikes ») avec le mot « kiki » et d’une forme arrondie avec le mot « bouba ».
Dans ce projet, nous allons faire l’hypothèse que cette association pourrait être due à une correspondance spectrale entre le son et l’image : en analyse phonétique, le spectre fréquentiel de « kiki » aura une fréquence fondamentale plus aigue que celui de « bouba ». ( voyelles diffuses/ compactes, consonnes sourdes/voisées)
De même, si l’on fait l’analyse spectrale (transformation de fourier 2D) des formes traditionnellement associées  à bouba et kiki dans la recherche (arrondies et épineuses/anguleuses), on s’aperçoit aussi que leurs spectres sont très différenciés. (fréquence fondamentale basse et peu d’harmoniques pour les formes rondes par exemple)
Notre expérience cherche donc à observer si le phénomène bouba-kiki peut être lié à une perception multi-modale du spectre fréquentiel, nous permettant d’extra-pôler l’étude à un stimuli auditif non linguistique qui en conserve les propriétés fréquentielles.
Le participant sera exposé en même temps que chaque son à deux images, dont l’une avec un spectre « congruent » et l’autre non, et devra sélectionner l’image qu’il choisit d’associer au son le plus intuitivement possible. Les temps de réponses seront mesurés, mais la donnée principale récoltée sera si l’association est « correcte » ou non c’est-à-dire si la ressemblance spectrale a été correctement détectée.

Contenu du répertoire : 

-	Un dossier images : Dans l’expérience on utilise seulement l’image « BoubaKiki » qui contient les deux images : Bouba se trouvant à Gauche et Kiki à Droite, le bouton appuyé par le participant devra correspondre à 275 : Gauche pour des sons B et 276 : Droite pour les sons K pour que l’association soit « correcte » (aille dans le sens de l’hypothèse de départ)
-	Un dossier /sons/ contenant 5 sons de chaque catégorie noté K pour Kiki et B pour Bouba 
-	Le dossier /data/ qui sera créé par expyriment pour ranger les fichiers individuels de résultats (numéro du participant, touche sélectionnée selon le stimulus, Temps de Réponse).
Consignes de  lancement du script :
Pour lancer le script il faut remettre le kernel à zéro (Restart & run all s’il a déjà été joué) car il semblerait qu’il se ferme  parfois mal s’il a déjà été joué mais je n’ai pas résolu le problème.

Pistes d’amélioration :

-	Si le principe de l’expérience est bien mis en place dans ce script, il manque en réalité une plus grande base de sons/ images, qu’on pourrait générer paramétriquement pour approfondir largement l’étude et l’analyse possible. Par exemple faire des catégories de sons avec des propriétés précises (attaque forte ou atténuée, tenue, écart de notes, harmoniques, etc.). On pourrait également imaginer décomposer spectralement des images de type Bouba ou Kiki et retransformer ce spectre en son (pour obtenir ainsi une correspondance « parfaite » image/son, et tester la sensibilité de l’association. Malheureusement j’ai vite abandonné cette idée au cours de mon projet car le bruit contenu dans les spectres rendait les sons 1. Très désagréables à l’oreille (rendant difficile pour un participant de supporter l’expérience) 2. difficilement distinguables à cause du bruit commun dans les images. Il aurait donc fallu passer beaucoup de temps à « nettoyer » les spectres obtenus (je n’ai pas ces compétences), ou à trouver une autre solution et j’ai donc préféré simplifier mes stimuli, tout en sachant qu’ils mériteraient d’être améliorés. Les sons sont donc simplement enregistrés sur un synthétiseur et leurs caractéristiques choisies arbitrairement parmis celles attribuées à Bouba ou Kiki en introduction.
-	De plus, il semble que la terminaison d’expérience d’expyriment ne laisse pas le kernel dans un état permettant de re-exécuter le programme : il est nécessaire de faire restart kernel pour recommencer, je n’ai pas réussi à comprendre pourquoi.

Retour sur expérience :

N’ayant jamais programmé auparavant j’ai été confrontée à un certain nombre de difficultés  lors de ce projet dont la manipulation des paths avec les chaînes Python et les caractères spéciaux, utiliser la documentation expyriment, pour par exemple afficher plusieurs images en même temps dans le stimuli avec la fonction ‘present()’, et j’ai donc utilisé des petits morceaux de code d’anciens projets ou trouvés sur le net en les modifiant ensuite pour les adapter à mon programme. Les difficultés rencontrées ne m’ont pas permis de créer un programme très ambitieux simplement d’abord à cause du temps utilisé à chercher/trouver/comprendre différentes fonctions puis à en changer, etc. Pour ma part j’ai trouvé le cours de PCBS un peu difficile d’accès pour les grands débutants, mais le format de projet aide à se confronter plus frontalement au code et donc à progresser à sa mesure et à commencer à prendre en main un langage, à s’habituer à la recherche de modules/fonctions sur le net etc.

