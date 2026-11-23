# Politique de confidentialité

Application « Ma Météo » (Android) · mise à jour le 23 novembre 2026

> **En bref :** l'application n'a ni compte, ni publicité, ni mesure d'audience. Le développeur n'a pas de serveur
> et ne reçoit aucune donnée. Pour afficher la météo, l'application demande les prévisions et la carte de pluie
> directement à trois services publics : Météo-France, Open-Meteo et l'IGN. Ces demandes contiennent le lieu
> choisi (ses coordonnées, ou le nom que vous cherchez) et, comme toute connexion à un site web, l'adresse IP de
> votre appareil.

## Ce que l'application garde sur votre appareil

- le dernier lieu choisi : son nom et ses coordonnées, pour le retrouver au prochain lancement ;
- le dernier écran ouvert (Prévisions ou Pluie).

Ces informations ne quittent pas l'appareil, sauf par la sauvegarde d'Android : si elle est activée, Android peut
les inclure dans la sauvegarde de votre compte Google, selon ses propres règles. Elles sont effacées quand vous
désinstallez l'application ou effacez ses données. Les prévisions reçues sont gardées en mémoire quelques minutes,
le temps de l'utilisation, et jamais enregistrées.

## Votre position

L'application ne demande la position de l'appareil que si vous touchez « Ma position ». Android vous demande
alors l'autorisation, la première fois. La position est lue une seule fois, à ce moment-là, sans chercher la
meilleure précision possible, et jamais en arrière-plan. Elle devient le lieu choisi : elle est gardée sur
l'appareil comme décrit plus haut, et envoyée aux services ci-dessous, avec une précision d'une dizaine de mètres,
pour obtenir le nom de la commune et les prévisions. Si vous refusez, rien d'autre ne change : vous pouvez
chercher une ville par son nom, et seules les coordonnées de cette ville sont alors envoyées.

## Les services appelés

Les demandes partent de votre appareil vers ces services, chiffrées (HTTPS), sans identifiant et sans passer par
le développeur. L'application n'appelle aucun autre serveur.

### Open-Meteo

`api.open-meteo.com`, `ensemble-api.open-meteo.com` et `geocoding-api.open-meteo.com` reçoivent les coordonnées
du lieu choisi, pour les prévisions (modèles de Météo-France et du Centre européen ECMWF), et le texte que vous
tapez dans la recherche, pour trouver les villes hors de France. Open-Meteo indique qu'il peut conserver les
adresses IP et les coordonnées demandées dans les journaux de ses serveurs, pour la maintenance et contre les
abus, et qu'il les efface au bout de 90 jours
([conditions et confidentialité d'Open-Meteo](https://open-meteo.com/en/terms#privacy)).

### IGN (Géoplateforme)

`data.geopf.fr`, le service public de l'Institut national de l'information géographique et forestière, reçoit :

- le texte que vous tapez dans la recherche, pour trouver les communes françaises ;
- votre position, si vous touchez « Ma position », pour trouver le nom de la commune ;
- les limites de la zone affichée sur la carte de pluie, pour en dessiner le fond.

Voir les [données à caractère personnel à l'IGN](https://www.ign.fr/institut/donnees-caractere-personnel).

### Météo-France

`public-api.meteofrance.fr` reçoit les limites de la zone affichée sur la carte de pluie : une région de quelques
centaines de kilomètres autour du lieu choisi, ou la France entière. Ces demandes portent la clé d'accès de
l'application, la même pour tous ses utilisateurs, qui ne vous identifie pas
([politique de confidentialité de Météo-France](https://meteofrance.com/politique-de-confidentialite)).

## Ce que l'application ne fait pas

- pas de compte, pas d'inscription ;
- pas de publicité, et pas d'identifiant publicitaire ;
- pas de mesure d'audience ni de rapport d'erreur envoyé ;
- aucune donnée vendue ni partagée par le développeur, qui n'en reçoit aucune.

## Enfants

Le développeur ne collecte aucune donnée, y compris de la part d'enfants.

## Modifications

Toute modification de cette politique sera publiée sur cette page, avec sa nouvelle date.

## Contact

Pour toute question : [maxou.houllier@gmail.com](mailto:maxou.houllier@gmail.com)
