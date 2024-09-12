```mermaid
  graph TD
    %% Acteurs
    acteur1[Utilisateur]
    acteur2[Administrateur]

    %% Cas d'utilisation
    uc1(Créer un compte)
    uc2(Se connecter)
    uc3(Supprimer un compte)
    uc4(Rechercher un film ou une série)
    uc5(Afficher les plateformes pour un film ou une série)
    uc6(Créer une watchlist)
    uc7(Ajouter un film à une watchlist)
    uc8(Supprimer une watchlist)
    uc9(Recommander l'abonnement le plus rentable)
    uc10(Gérer les tiers d'abonnements)
    uc11(Gérer la localisation de l'utilisateur)

    %% Relations entre les acteurs et les cas d'utilisation
    acteur1 -- Créer un compte --> uc1
    acteur1 -- Se connecter --> uc2
    acteur1 -- Supprimer un compte --> uc3
    acteur1 -- Rechercher un film ou une série --> uc4
    acteur1 -- Afficher les plateformes pour un film ou une série --> uc5
    acteur1 -- Créer une watchlist --> uc6
    acteur1 -- Ajouter un film à une watchlist --> uc7
    acteur1 -- Supprimer une watchlist --> uc8
    acteur1 -- Recommander l'abonnement le plus rentable --> uc9
    acteur1 -- Gérer la localisation de l'utilisateur --> uc11

    acteur2 -- Gérer les tiers d'abonnements --> uc10
    acteur2 -- Recommander l'abonnement le plus rentable --> uc9

    %% Extension (facultatif)
    uc9 --> uc10 : << optionnel >>
    uc9 --> uc11 : << optionnel >>
```
