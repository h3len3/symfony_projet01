# Description du projet symfony                                 Hélène - WAD23


## Site pour une professeure de yoga avec
   ↪ d’une part,  une partie statique des pages qui informent sur elle et le yoga, 
   ↪ et d’autre part,  une partie dynamique qui est un agenda permettant de gérer les inscriptions aux cours individuels et aux matinées yoga.

## La prof propose:
- des cours collectifs hebdomadaires de yoga à horaires réguliers (inscription une fois par an. Exemple: inscriptions possibles jusqu’au 05 septembre).
- des cours individuels 
- des matinées de yoga 
- des évènements de type autres (par exemples séance de chant)

## 3 cas d’utilisation : un visiteur non inscrit au site, un utilisateur inscrit et du point de vue du prof de yoga

    ### visiteur non inscrit au sens pas de compte sur le site :
    - peut naviguer sur les pages pour s'informer sur le prof, le yoga et voir l'agenda
    - peut s'inscrire au sens créer un compte sur  le site 
     

    ### L'utilisateur inscrit
    - peut naviguer sur les pages pour s'informer sur le prof, le yoga et voir l'agenda
    - (peut se déinscrire au sens supprimer son compte? utile?)

    - peut s'inscrire aux cours collectifs hebdomadaire (si les inscriptions sont encore ouvertes et si il y a encore une place disponibles) 
    - peut s’inscrire à des cours individuels (si il s’inscrit endéans 24H avant le rdv) 
    - peut s’inscrire à des matinées yoga (si une place est encore disponible) 
    - peut s’inscrire à des événements de type autres (si une place est encore disponible) 
  
    - peut annuler son inscription aux cours collectifs si la date pour les inscriptions aux cours collectifs n’est pas passée. 
          Pour les cours collectifs, je vais partir de la base que normalement il y a une date de début d’inscription et une date de limite d’inscription et que une fois celle-ci dépassée, le membre ne peut plus s’incrire ni se désinscrire par lui-même via l’agenda en ligne. 
                 Pour se désinscrire ou pour se désinscrire une fois  la date passée / les cours commencés, on laisse une possibilité : si un membre est dans une de ces situations, il le dit à la prof et/ou envoit un mail, et la prof peut agir sur l’appli -> peut inscrire ou désinscrire le membre. 
                              Niveau “publique”, on les voit toujours dans les agenda même publique, mais on peut pas plus s'inscrire ou de désinscrire après la date limite
                        Que faire avec les places dispo ?  A partir de la date de clôture, elles n’apparaissent plus
                      + laisser la possibilité au prof de commenter (si elle voulait quand même mettre “il reste 1 place disponible… si intéressé, envoyer un mail”) (-> si ça va pas, le mettre dans nom ? )

     - peut annuler sa réservation pour un cours individuel (endéans un certain délai ? )
     - peut annuler sa réservation d’une place à une matinée de yoga et un évenement de type autre (endéans un certain délai?)

     - Depuis une page sur son compte sur le site, il peut visualiser tout ce dont à quoi il est actuellement inscrit 
     (aspect : liste + si temps petit agenda à coté. Si pas le temps, que liste)

    ### Coté prof
- peut ajouter des cours collectifs, des cours individuels, des matinées yoga, des évenements de type autre 
  + modifier et supprimer
    Quand modification ou suppression d’un évenement au sens large -> mail aux membres concernés cfr ligne 65 
    Peut commenter un évenement (= je pense que =modifier?)
- peut inscrire et désinscrire quelqu’un d'un évenement au sens large
- peut inscrire et désinscrire quelqu’un du site
   

## Pour les cours collectifs et les matinées : le nombre de place(s) disponible(s) 
- Le nombre de place(s) disponible(s) varie automatiquement selon que des personnes s’inscrivent ou annulent. → pour les cours co et matinées et autres évenements.
- Pour les cours individuels, il “disparait” de l’agenda “publique” et vu par membres puisque la plage n’est plus disponible. 

## Système de mails de confirmation (d'inscription, d’annulation), de rappel, d’ “alerte”, et éventuellement d’annonce : 
- Pour les utilisateurs : ⬝ mails de confirmation à chaque réservation 
                                                et à chaque annulation 
                        ⬝ mail de rappel s’envoyant
                                 la veille du premier cours de cours collectifs hebdomadaire,  
                                 la veille de chaque cours individuels 
                                et la veille de chaque matinée de yoga et de évenement de type autres
                          → aux personnes inscrites à cela

- Quand la prof annule ou modifie un événement, un mail est envoyé aux membres inscrits à celui-ci pour les informer.

- (Quand la prof ajoute à l’agenda un évenement (au sens large), un mail est envoyé à tous les membres pour les informer de cet ajout. (NB : Attention à ce que celui peut créer si elle revoit d’un coup son planning et ajoute plein de plages cours individuel par exemple , ou même cours co)) + NB : pas prioritaire

- Quand un utilisateur réserve, quand un utilisateur annule, un mail s’envoit automatiquement à la prof pour l’informer


## Agendas, différentes versions 
A. publique (visible sur le site pour les visiteurs qui n’ont pas un compte)
B. publique; membres -> même que le premier normalement

C. membre espace perso (son perso): une liste + éventuellement si temps un petit agenda cfr lignes 40 et 41

D. du prof 


