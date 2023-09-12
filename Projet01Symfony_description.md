Description du projet symfony                                 Hélène - WAD23


Site pour une professeure de yoga avec
   ↪ d’une part,  une partie statique des pages qui informent sur elle et le yoga, 
   ↪ et d’autre part,  une partie dynamique qui est un agenda permettant de gérer les inscriptions aux cours individuels et aux matinées yoga.

La prof propose:
- des cours collectifs hebdomadaires de yoga à horaires réguliers (inscription une fois par an. Exemple: inscriptions possibles jusqu’au 05 septembre).
- des cours individuels 
- des matinées de yoga 

2 cas d’utilisation : du point de vue d’un utilisateur et du point de vue du prof de yoga : 

    L'utilisateur
       - peut naviguer sur les pages pour s'informer sur le prof, le yoga et voir l'agenda

       - peut s'inscrire au sens créer un compte sur  le site 

       - peut s'inscrire aux cours collectifs hebdomadaire (si les inscriptions sont encore ouvertes et si il y a encore une place disponibles) → Pour ce faire, il doit avoir un compte sur le site 
       - peut s’inscrire à des cours individuels (si il s’inscrit endéans 24H avant le rdv) → Pour ce faire, il doit avoir un compte sur le site 
       - peut s’inscrire à des matinées yoga (si une place est encore disponible) → Pour ce faire, il doit avoir un compte sur le site 
  
       - peut annuler son inscription aux cours collectifs si la date pour les inscriptions aux cours collectifs n’est pas passée. Si oui, ça sera possible mais via mail (car soit ça serait la veille de début des cours soit et généralement alors que il y a déjà eu un ou des cours donc discussions avec prof sur remboursements  prorata, etc (NB: Je dois parler avec la prof de ce qu’elle fait exactement dans ce cas)
     - peut annuler sa réservation pour un cours individuel 
     - peut annuler sa réservation d’une place à une matinée de yoga.

     - Depuis une page sur son compte sur le site, il peut visualiser tout ce dont à quoi il est actuellement inscrit.

    Coté prof
      -  peut ajouter des cours collectifs, des cours individuels, des matinées yoga + modifier et supprimer
      - quand modification ou suppression d’un cours ou d’une matinée -> mail aux membres concernés 


Pour les cours collectifs et les matinées : le nombre de place(s) disponible(s) :
Le nombre de place(s) disponible(s) varie automatiquement selon que des personnes s’inscrivent ou annulent.

Système de mails de confirmation (d'inscription, d’annulation), de rappel, d’ “alerte”) : 
  - Pour les utilisateurs : ⬝ mails de confirmation à chaque réservation, mais de confirmation à chaque annulation, 
                        ⬝ mail de rappel s’envoyant la veille du premier cours de cours collectifs hebdomadaire,  la veille de chaque cours individuels et la veille de chaque matinée de yoga)
  - Quand un utilisateur réserve, quand un utilisateur annule, un mail s’envoit automatiquement au prof pour l’informer

