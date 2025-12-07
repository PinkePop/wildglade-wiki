---
hide:
  - navigation
  - toc
  - footer
---

# Règles { align=center }

=== "Déplacement"

    Le déplacement se fait à chaque tour, en lançant un D10. Le résultat détermine à la fois la direction et le nombre de cases parcourues.

    ## Direction

    Si le résultat est impair, le déplacement s'effectue en diagonal.

    Si le résultat est pair, le déplacement s'effectue en ligne droite.

    ## Règles de déplacement

    - Le joueur choisit une direction initiale.
    - Il avance tout droit jusqu'à consommer entièrement le déplacement.
    - Il ne peut tourner que lorsqu'il heurte un mur.
    - Toutes les cases traversées appliquent leurs effets.
    - Une toile d'araignée nécessite +1 déplacement supplémentaire pour être franchie.

=== "Caractéristiques"

    Chaque personnage possède cinq caractéristiques :

    - Force (FOR) : puissance brute, utilisé pour les jets avec les armes lourdes.
    - Agilité (AGI) : vitesse, utilisé pour les jets avec les armes courtes et distance.
    - Endurance (END) : robustesse, point de vie.
    - Intelligence (INT) : maîtrise des sorts, utilisé pour les jets de magie.
    - Charisme (CHA) : chance sur les échecs critiques, les coffres et les gains d'or.
  
    Le joueur commence avec un point dans chacune de ces caractéristiques à l'exception du charisme qui est à 0.

    Aucune statistique ne peut dépasse 16.

=== "Point de Vie"

    Les PV d'un personnage dépendent directement de son endurance.

    ```
    PV MAX = 10 + (END x 3)
    ```

    Augmenter l'endurance permet d'augmenter immédiatement les PV Max et également les PV actuels.

    Par exemple: si j'ai 19PV avec un maximum à 23, ajouter un point dans l'endurance permet d'augmenter son maximum à 26, et de soigner 1 PV. Je passe donc à 20PV/26.

=== "Points de compétence"

    À chaque étage réussi, le joueur gagne 1 point de compétence.

    Ce point peut etre investi dans n'importe quelle caractéristique, dans la limite du maximum du cap de 16.

    Les étages 46 à 50 ne donnent pas de points, car ils correspondent à la zone finale.

=== "Mécaniques de Jet"

    Chaque combat se base sur un jet d'opposition entre le joueur et la créature.

    ## Jet d'Opposition

    Chacun lance 1D20. Un jet est réussi si D20 <= Caractéristiques utilisée.

    ### Quelle caractéristique utiliser ?

    - Arme lourde : Force
    - Arme courte : Agilité
    - Arme à distance : Agilité
    - Sort et Parchemin : Intelligence
      - Exception : un non-Mage lance avec INT +2.

    ### Calcul de la Réussite

    ```
    Réussite = Caractéristique - Résultat du D20.
    ```

    Plus le résultat est bas, plus la réussite est élevée.

    ## Détermination du vainqueur du jet

    Le combattant ayant la réussite la plus élevée inflige des dégâts. La réussite peut être négative.

    ## Dégâts

    ```
    Dégâts = ((Ecart des réussites) + Dégâts de l'Arme + Bonus ATK) - Armure adverse
    ```

    ## Critiques

    ### Réussite critique

    Si le résultat du dé est à 1, c'est une réussite critique. La réussite ennemie est ignorée.

    La réussite est considérée à 1. Cependant, les dégâts seront doublés.

    ### Echec critique

    Si le résultat du dé est 20, c'est un échec critique. En cas d'échec critique, le joueur a :

    - 30% de chance que son arme se brise, ou que le sort soit oublié (pour un Mage).
    - 65% de chance que les dégâts subi soit augmenté de 1.
    - 5% de chance que le critique n'ait pas de conséquence.

    ### Rôle du charisme

    Chaque point de charisme augmente de 1% la probabilité d'obtenir "aucune conséquence" lors d'un échec critique.

    Il réduit d'abord la probabilité de casse, puis celle du dégâts bonus.

    Par exemple, avec 5 points de charisme :

    - 25% de chance que son arme se brise, ou que le sort soit oublié (pour un Mage).
    - 65% de chance que les dégâts subi soit augmenté de 1.
    - 10% de chance que le critique n'ait pas de conséquence.