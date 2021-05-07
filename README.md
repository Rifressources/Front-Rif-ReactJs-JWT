 Ce Projet est un exemple d'authentification JWT avec  React.js: login  et enregistrement avec:
 
       -LocalStorage
 
      -React Router
 
       -Axios 
 
       -Bootstrap 
 
 Notre application ReactJS  peut être résumée dans le diagramme ci-dessous :
 
 
 ![ReactProject](https://user-images.githubusercontent.com/81759205/117468117-a7aa4680-af54-11eb-9c6f-c032850394a4.png)


- Le composant  App est un conteneur avec React Router ( BrowserRouter). En fonction de statel, la barre de navigation peut afficher ses éléments.
- Les composants Login & Registeront  ont un formulaire  pour la soumission des données (avec le soutien de la bibliothèque react-validation). Ils appellent les méthodes de auth.service pour faire une demande de connexion / d'enregistrement.
-Les méthodes auth.service utilisent axios pour effectuer des requêtes HTTP. Il stocke ou récupère également JWT à partir du stockage local du navigateur dans ces méthodes.
- Le composant Home est public pour tous les visiteurs.
- Le composant  Profile affiche les informations de l'utilisateur une fois l'action de connexion réussie.
- Les  composants BoardUser, BoardModerator, BoardAdminseront affichés par state  user.roles. Dans ces composants, nous utilisons user.service pour accéder aux ressources protégées à partir de l'API Web.
- user.service utilise la fonction  auth-header() d'assistance pour ajouter JWT à l'en-tête HTTP. auth-header() renvoie un objet contenant le JWT de l'utilisateur actuellement connecté à partir du stockage local.





 
 
