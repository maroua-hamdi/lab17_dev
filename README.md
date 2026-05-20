# LAB 17 : Maîtriser les BroadcastReceiver en Android

## Informations du lab

- Cours : Programmation Mobile
- Technologie : Android avec Java
- Sujet : BroadcastReceiver
- Application réalisée : ReceiverDemo
- Réalisé par : HAMDI Maroua

---



## Objectif du lab

Ce lab a pour objectif de comprendre le fonctionnement des BroadcastReceiver en Android.

Un BroadcastReceiver est un composant Android qui permet à une application de recevoir et de traiter des événements envoyés par le système Android ou par l’application elle-même.

Dans ce lab, nous avons réalisé une application Android appelée ReceiverDemo. Cette application permet de tester l’utilisation des BroadcastReceiver à travers une interface simple.

L’application permet notamment de :

- détecter le changement du mode avion ;
- utiliser un Receiver dynamique ;
- envoyer un Broadcast interne personnalisé ;
- afficher un message Toast après l’envoi du Broadcast.

---

## Description de l’application

L’application affiche une interface simple contenant :

- un message principal ;
- un bouton pour désactiver le Receiver du mode avion ;
- un bouton pour envoyer un Broadcast interne ;
- un message Toast en bas de l’écran après l’envoi du Broadcast.

Dans la capture finale, on peut voir le message suivant :

Airplane receiver enabled

Cela signifie que le Receiver du mode avion est activé.

---

## Fonctionnalités réalisées

### 1. Receiver dynamique

Un Receiver dynamique a été utilisé pour détecter le changement du mode avion.

Ce type de Receiver est déclaré directement dans le code Java, généralement dans l’Activity principale.

Il est utile lorsque l’on veut écouter un événement uniquement pendant que l’application est active.

---

### 2. Bouton de désactivation du Receiver

Le bouton suivant est présent dans l’application :

Disable Airplane Receiver

Ce bouton permet de désactiver le Receiver dynamique lié au mode avion.

Cela montre que le Receiver peut être contrôlé directement depuis l’interface de l’application.

---

### 3. Broadcast interne personnalisé

Le deuxième bouton affiché est :

Send Internal Broadcast

Lorsque l’utilisateur clique sur ce bouton, l’application envoie un Broadcast interne personnalisé.

Après l’envoi du Broadcast, un message Toast apparaît en bas de l’écran.

---

### 4. Affichage du Toast

Après le clic sur le bouton Send Internal Broadcast, le message suivant s’affiche :

Internal broadcast sent

Ce message confirme que le Broadcast interne a bien été envoyé.

---

## Étapes de réalisation

### Étape 1 : Création du projet Android

Un nouveau projet Android a été créé avec Java.

Le projet a été nommé ReceiverDemo.

L’objectif était de créer une application simple permettant de tester les BroadcastReceiver.

---

### Étape 2 : Création du Receiver dynamique

Un BroadcastReceiver dynamique a été créé dans l’Activity principale.

Ce Receiver permet d’écouter l’événement lié au changement du mode avion.

L’action utilisée est :

ACTION_AIRPLANE_MODE_CHANGED

---

### Étape 3 : Enregistrement du Receiver

Le Receiver dynamique a été enregistré dans le code de l’Activity.

Cela permet à l’application de recevoir les événements pendant son exécution.

---

### Étape 4 : Ajout du bouton de désactivation

Un bouton a été ajouté pour désactiver le Receiver dynamique.

Ce bouton permet de mieux comprendre le cycle de vie d’un BroadcastReceiver dynamique.

---

### Étape 5 : Création du Broadcast interne

Un Broadcast personnalisé a été ajouté dans l’application.

Ce Broadcast est envoyé lorsque l’utilisateur clique sur le bouton Send Internal Broadcast.

---

### Étape 6 : Affichage du message Toast

Après l’envoi du Broadcast interne, un Toast est affiché pour confirmer l’action.

Le message affiché est :

Internal broadcast sent

---

### Étape 7 : Test sur l’émulateur

L’application a été testée sur un émulateur Android.

Le résultat final est visible dans la capture suivante :

<img width="388" height="755" alt="image" src="https://github.com/user-attachments/assets/44fd8894-7168-45b5-9086-ec4326f39c3c" />


Dans cette capture, on remarque que :

- l’application se lance correctement ;
- le message principal est affiché ;
- les deux boutons sont visibles ;
- le Toast apparaît correctement en bas de l’écran.

---

## Résultat obtenu

Le résultat final montre que l’application fonctionne correctement.

L’interface affiche :

Airplane receiver enabled

Les deux boutons sont présents :

Disable Airplane Receiver

Send Internal Broadcast

Et le message Toast s’affiche après l’envoi du Broadcast :

Internal broadcast sent

Cela confirme que le Broadcast interne a été envoyé avec succès.

---

## Différence entre Receiver dynamique et Receiver statique

Un Receiver dynamique est déclaré dans le code Java. Il fonctionne généralement lorsque l’application est ouverte ou lorsque l’Activity est active.

Un Receiver statique est déclaré dans le fichier AndroidManifest.xml. Il peut recevoir certains événements système même si l’application n’est pas ouverte, selon les restrictions Android.

Dans ce lab, l’accent principal est mis sur le Receiver dynamique et le Broadcast interne personnalisé.

---

## Conclusion

Ce lab m’a permis de comprendre le rôle des BroadcastReceiver dans Android.

J’ai appris à :

- créer un BroadcastReceiver dynamique ;
- écouter un événement système ;
- désactiver un Receiver depuis l’interface ;
- envoyer un Broadcast interne personnalisé ;
- afficher un Toast après une action ;
- tester le fonctionnement de l’application sur un émulateur Android.

Les BroadcastReceiver sont importants dans Android car ils permettent à une application de réagir automatiquement à des événements du système ou à des événements internes.

---

## Auteur

Réalisé par :

HAMDI Maroua
