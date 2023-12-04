---
Author:
    - Alexis Opolka
    - Mathys Domergue
    - Thibault Garcia
Company: IUT de Béziers
Subject: Cas d'Etude d'installation FO
Copyright: All Rights Reserved

Header:
    Left: Alexis O., Mathys D., Thibault G.
Footer:
    Center: "&copy; {{ ChangeDate 'yyyy' }} {{ Author }} - {{ Copyright }}"
---

# SAE-31 - Un cas d'étude

## Sujet

Ce projet est monté autour de la SAE-301 (aussi appelée SAE-31 sur ce dépôt) dont le PN est accessible [ici](https://github.com/alexis-opolka/vert/blob/main/src/PN-SAE301.pdf),
où le sujet est de faire un cas d'étude sur l'installation d'une desserte fibrée dans une zone nouvellement constructible en périphérie de la ville de Rouen.  
Nous devons principalement faire la desserte d'un [immeuble de standing](https://www.bnppre.fr/glossaire/immeuble-de-standing.html) comportant 7 logements,
en plus de cela, il nous est demandé de préparer le raccordement d'emplacements déjà prévus à la construction afin de faciliter leur futur installation.

## Contexte et Hypothèses de base

### Contexte de base

Comme cité précédemment, nous nous situons en périphérie de [Rouen](https://maps.app.goo.gl/9QaDGt49Um4JFxcUA) dans une zone nouvellement constructible et sommes
dans une zone boisée, nous avons donc décidé de caractériser la zone de construction comme une zone peu dense (soit ZMD ou Zone Moins Dense).

Nous avons, en soit, 4 zones à desservir:

- L'immeuble de standing de 7 logements
- Un site dans une zone boisée de 12 futurs logements
- Un site plus "en haut" du plan cadastral de 8 logements, se trouvant en dehors de la zone boisée
- Deux sites de 18 logements chacun près d'une route déjà construite plus "en bas" du plan cadastral

Ce qui nous fait un total de $7 + 12 + 8 + 18 \times 2 = 63$ logements à desservir.

![carte-depart](./src/scan-carte-depart.jpeg)

Nous avons constaté deux défis principaux dans ce contexte.  
Le premier étant de desservir la zone nouvellement constructible dans l'espace boisé et le deuxième se trouve être
de prévoir les futures voies d'accès et les autres raccordements (eau, éléctricité, etc.) pour les zones nouvelles constructibles.

### Hypothèses de base

- #### Des liens aériens

    Nous avons donc décidé de partir sur une majorité de liens aériens.  
    Ils se trouvent être plus susceptibles aux dommages causés par la nature, mais dans notre cas, si l'espace boisé qui les entoure
    ne vient pas à disparaitre sur du court terme, les arbres permettront d'absorber une partie des vents forts et leurs racines
    permettront de stabiliser le sol à proximité des fondations des structures de support rendant ainsi le sol à proximité moins
    vulnérable.

- #### Des raccordements FO ultérieurs ou déjà présents

    Nous avons supposé que la partie des raccordements jusqu'au client serait soit déjà présente ou serait mise en place
    ultérieurement durant, voir après la construction des logements.

    Ceci nous permettant donc de ne pas se concentrer sur les aspects de raccordements au sein d'un batiment et
    plus sur la desserte globale de la zone enlevant par extension des coûts propres à ces installations.

- #### Des raccordements de nécessité déjà préparés

    On considère le raccordement en eau et en électricité des raccordements de `nécessité`,
    ainsi donc, on considère qu'une société à part entière s'est déjà occupé de les effectuer
    ou de préparer les raccordements.

    Ceci nous permettant de nous concentrer seulement sur le raccordement Fibre Optique.

## Une société fictive

Afin d'organiser ce projet (et essayer de l'ammener au plus proche de la réalité), nous avons décidé de créer une société fictive du nom de <span class="sae31Vert">Vert</span>, inspiré de la
société française [Orange](https://orange.com), sa dénomination tout le long du projet sera `Vert SA` ou `Vert, une Société Anonyme`.

## Auteurs

Ce travail a été effectué et vous est proposé par [Alexis Opolka](https://github.com/alexis-opolka), [Mathys Domergue](https://github.com/Mathys-Domergue)
et [Thibault Garcia](https://github.com/ThibaultGarcia), durant leur cursus de 2ème année de BUT Réseaux et Télécommunications à [l'IUT de Béziers](https://iutbeziers.fr).

<div>

## Méthode de travail et gestion de projet

Nous avons décidé de regrouper tout notre travail sur un dépôt GitHub, que vous pouvez retrouver [ici](https://github.com/alexis-opolka/Vert/).  
Pour la gestion de projet, nous avons utilisé un Kaban, disponible sur le GitHub Projects, accessible [via ce lien](https://github.com/users/alexis-opolka/projects/4/views/1).

## Compte-rendu
