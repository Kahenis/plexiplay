# Plexiplay

**Plexiplay** est une application pour regarder vos films et séries **Plex** sur une télévision ou une box **Android TV** (Orange, Chromecast avec Google TV, Nvidia Shield, Sony, Philips, etc.), entièrement pensée pour la télécommande.

Elle n'est pas dans le Play Store : on l'installe une seule fois à partir de ce dépôt. Ensuite, elle se met à jour toute seule.

> Ce dépôt est un **dépôt de distribution** : il contient les APK (onglet [Releases](https://github.com/Kahenis/plexiplay/releases)) et cette documentation. Le code source n'est pas publié.

**[⬇ Télécharger la dernière version](https://github.com/Kahenis/plexiplay/releases/latest)**

## Sommaire

- [Ce qu'il vous faut](#ce-quil-vous-faut)
- [Installation](#installation)
  - [Méthode A : clé USB et CX Explorer (la plus facile)](#méthode-a--clé-usb-et-cx-explorer-la-plus-facile)
  - [Méthode B : Downloader for TV](#méthode-b--downloader-for-tv)
  - [Méthode C : AnExplorer (moins facile)](#méthode-c--anexplorer-moins-facile)
  - [Après la première installation](#après-la-première-installation)
- [Première connexion](#première-connexion)
- [Mode d'emploi](#mode-demploi)
- [Les réglages](#les-réglages)
- [Un problème ? Quel réglage essayer](#un-problème--quel-réglage-essayer)
- [Questions fréquentes](#questions-fréquentes)
- [Ce qui viendra plus tard](#ce-qui-viendra-plus-tard)
- [Signaler un problème](#signaler-un-problème)

## Ce qu'il vous faut

- une TV ou une box **Android TV** connectée à internet, et sa télécommande ;
- un compte **Plex** (gratuit) avec accès à un serveur Plex, le vôtre ou celui d'un ami.

Pour installer : une clé USB et un ordinateur ou un téléphone (méthode A), ou rien de plus (méthode B).

## Installation

Au moment de l'installation, Android bloque une application qui ne vient pas du Play Store, par sécurité. Un message « Pour votre sécurité, l'installation est bloquée » s'affiche, avec un bouton **Paramètres** : il suffit d'activer l'interrupteur, puis d'appuyer sur **Retour**. Cette autorisation ne se donne qu'une seule fois.

Vous verrez peut-être aussi le message « Nous n'avons pas d'antécédents pour ce développeur, nous conseillons de ne pas installer cette application ». Vous passez outre l'avis et choisissez **« installer quand même »** 😊. Ce message ne s'affiche lui aussi qu'une seule fois.

Selon votre télévision et la version d'Android, les menus peuvent avoir un nom ou un aspect légèrement différent de ce qui est décrit ci-dessous.

### Méthode A : clé USB et CX Explorer (la plus facile)

Pour une première installation, c'est de loin la méthode la plus facile : aucune adresse à taper avec la télécommande. Il suffit de copier le fichier de Plexiplay sur une clé USB, puis de l'ouvrir depuis la TV avec un gestionnaire de fichiers gratuit, **CX Explorer** (aussi appelé CX Explorateur). La TV doit avoir un port USB.

1. **Installez CX Explorer** depuis le store de la TV : ouvrez le Google Play Store, cherchez « CX Explorer » (ou « CX Explorateur »), puis choisissez **Installer**.
2. **Téléchargez l'APK** sur votre ordinateur ou votre téléphone, depuis la [page des versions](https://github.com/Kahenis/plexiplay/releases/latest) (fichier `PlexiPlay-x.y.z.apk` dans la section *Assets*), puis copiez-le sur la clé USB.
3. **Insérez la clé USB** dans un port USB de la télévision ou du boîtier.
4. **Ouvrez CX Explorer**, autorisez la gestion des fichiers (bouton *Autoriser* au premier lancement), sélectionnez la clé USB, puis le fichier `.apk`, et appuyez sur **OK**.
5. **Autorisez CX Explorer à installer des applications** : Android affiche un message de sécurité avec un bouton *Paramètres* ; activez l'interrupteur pour CX Explorer, puis appuyez sur **Retour**.
6. **Confirmez l'installation** : Android demande « Voulez-vous installer cette application ? ». Descendez jusqu'à **Installer**, puis **OK**. À la fin, choisissez **Ouvrir**, ou retrouvez l'icône Plexiplay dans le menu de la TV. Vous passez alors à la [connexion](#première-connexion).

Vous n'avez pas de clé USB ? Utilisez la méthode B.

### Méthode B : Downloader for TV

Si vous n'avez pas de clé USB, c'est la méthode la plus simple : **Downloader for TV** est une petite application pensée pour la télécommande. Elle télécharge un fichier à partir d'une adresse internet, puis l'installe directement.

1. **Installez « Downloader for TV »** depuis le Play Store de la TV (utilisez la loupe). Respectez bien le nom *Downloader for TV* : il existe deux autres logiciels « downloader » nettement moins pratiques.
2. **Ouvrez-le et acceptez les autorisations.** Au premier lancement, l'application demande l'accès aux fichiers : choisissez **Autoriser**. Si l'écran « Sources inconnues » apparaît, activez l'interrupteur.
3. **Saisissez l'adresse de la page des versions**, sans toucher aux cases optionnelles. Dans la zone de saisie (sélectionnez-la avec les flèches pour faire apparaître le clavier), tapez :

   ```
   github.com/Kahenis/plexiplay/releases/latest
   ```

   Appuyez sur **DOWNLOAD** (le bouton peut aussi s'appeler *Télécharger*, *GO* ou *OK* selon la version), puis sur la page qui s'affiche descendez jusqu'au fichier `PlexiPlay-x.y.z.apk` de la section *Assets* et validez avec **OK**.
4. **Attendez la fin du téléchargement.** Une barre de progression s'affiche ; cela prend quelques instants selon votre connexion.
5. **Choisissez « Install ».** Android affiche « Voulez-vous installer cette application ? » : descendez jusqu'à **Installer**, puis **OK**. La TV peut vous demander de valider l'autorisation d'installation de Downloader for TV.
6. **Ouvrez Plexiplay.** À la fin, retournez au menu Android et cliquez sur l'icône Plexiplay. Downloader for TV peut proposer de supprimer le fichier téléchargé : répondez **Supprimer**, vous n'en avez plus besoin.

### Méthode C : AnExplorer (moins facile)

AnExplorer est un gestionnaire de fichiers qui sait aussi télécharger depuis internet. Choisissez cette méthode uniquement si ni CX Explorer ni Downloader for TV ne sont disponibles sur votre TV.

1. Installez **AnExplorer** depuis le Play Store de la TV.
2. Ouvrez-le, acceptez les autorisations demandées, puis activez « Sources inconnues » pour AnExplorer si la TV le demande.
3. Dans le menu de gauche, ouvrez la section réseau ou téléchargement (son nom varie selon la version), puis saisissez l'adresse `github.com/Kahenis/plexiplay/releases/latest` et téléchargez le fichier `PlexiPlay-x.y.z.apk`.
4. Allez dans *Téléchargements*, sélectionnez le fichier avec la télécommande, puis **OK**.
5. Choisissez **Installer**, puis **Ouvrir** : c'est la même confirmation que dans les méthodes A et B.

### Après la première installation

Vous n'aurez plus à refaire ces étapes : Plexiplay vérifie seul à chaque démarrage s'il existe une nouvelle version, et vous la propose. Vous pouvez aussi la vérifier à la main dans **Paramètres → Recherche mise à jour**, puis choisir **Mise à jour**.

Pour installer une version précise, ou si une mise à jour ne se propose pas, téléchargez simplement l'APK voulu dans la [liste des versions](https://github.com/Kahenis/plexiplay/releases) et installez-le par-dessus la version existante (vos réglages sont conservés).

## Première connexion

Dans la liste des applications de la TV, ouvrez **Plexiplay**. Un écran de démarrage avec une barre de progression s'affiche pendant que l'application charge vos bibliothèques.

**Connexion avec un code** (recommandée) : la première fois, Plexiplay vous demande de lier la TV à votre compte Plex, comme pour les autres applications Plex.

1. Notez le **code à 4 caractères** affiché en grand au centre de l'écran.
2. Sur votre téléphone ou votre ordinateur, allez sur **plex.tv/link**, connectez-vous à votre compte Plex si on vous le demande, puis saisissez le code.
3. Attendez quelques secondes : la TV détecte toute seule que le code est validé et passe à l'Accueil.

Le code expire au bout de quelques minutes : si besoin, choisissez **Nouveau code** avec la télécommande.

**Connexion classique** : vous tapez votre identifiant Plex et votre mot de passe avec le clavier de la TV, puis **Valider**. C'est un peu plus long avec une télécommande, d'où la préférence pour le code.

**Quel serveur est utilisé ?** Plexiplay choisit automatiquement un serveur qui contient des films ou des séries. Si vous avez le vôtre et que des amis vous en partagent un, vous les retrouvez tous dans les paramètres (ligne *Serveur*) et pouvez passer de l'un à l'autre à tout moment.

**Si la connexion ne fonctionne plus.** Quand Plex ne reconnaît plus votre session (par exemple après avoir retiré l'appareil depuis votre compte plex.tv), Plexiplay vous ramène tout seul à l'écran de connexion, avec un message « Votre session Plex a expiré. Veuillez vous reconnecter. » : il suffit de refaire un code. Si c'est le serveur qui est injoignable (éteint, ou TV sans internet), un écran l'explique simplement et propose **Réessayer** ou **Se reconnecter**.

## Mode d'emploi

> Se déplacer : **flèches** pour naviguer, **OK** pour choisir, **Retour** pour revenir en arrière. Depuis le contenu, Retour ramène d'abord à l'onglet précédent, puis au menu de gauche.

### Le menu de gauche

Toute l'application s'organise autour du menu de gauche. Il est réduit (icônes seulement) quand vous naviguez dans le contenu, et se déploie avec les noms quand vous revenez dessus.

| Ligne | Ce qu'elle ouvre |
|---|---|
| Accueil | Un résumé : ce que vous regardiez, les nouveautés, etc. |
| Recherche | Trouver un film ou une série par son titre. |
| Vos bibliothèques (Films, Séries…) | Chacune a ses propres onglets. |
| Roue crantée (en haut) | Les paramètres. |

L'ordre des bibliothèques (menu de gauche et Accueil) place toujours vos films en premier, vos séries juste après, puis le reste (documentaires, dessins animés, concerts…) par ordre alphabétique.

### L'Accueil

L'Accueil rassemble, bibliothèque par bibliothèque, deux rangées d'affiches : **« <bibliothèque> - Continuer à voir »** et **« <bibliothèque> - Derniers ajouts »**. Flèches gauche/droite pour les parcourir, haut/bas pour changer de rangée. Une bibliothèque n'apparaît sur l'Accueil que si elle est à la fois affichée dans le menu de gauche (réglage *Bibliothèques affichées*) et autorisée pour l'accueil côté serveur Plex (réglage Plex *Gérer les recommandations*) ; une rangée sans aucun contenu ne s'affiche pas.

- **Continuer à voir** : ce que vous avez commencé, du plus récent au plus ancien. Un épisode apparaît avec l'affiche de la série et une étiquette orange « S2 · E5 » (saison 2, épisode 5).
- **Derniers ajouts** : les nouveautés de cette bibliothèque, du plus récent au plus ancien. Quand plus de 4 épisodes d'une même saison sont ajoutés d'un coup, ils sont regroupés en **une seule affiche** avec un bandeau orange « 8 ajouts » ; un clic ouvre directement la page de cette saison.
- **Retirer un titre de « Continuer à regarder »** : placez-vous sur l'affiche et maintenez **OK** environ 3 secondes, puis choisissez *Supprimer de « Continuer à regarder »*. Même chose pour « Regarder à nouveau ».

### Les onglets d'une bibliothèque

Quand vous ouvrez une bibliothèque (par exemple « Films »), des onglets apparaissent en haut :

- **Bibliothèque** : tous les titres ;
- **Collections** : regroupements (films uniquement) ;
- **Style** : parcourir par genre, humour, action, drame… (films et séries) ;
- **Quoi de neuf** : nouveautés, plus regardés, à revoir ;
- **Idée TV** : tout à droite, pour obtenir 5 idées de films au hasard (films uniquement).

**Nombre de films et interrupteur « Sagas ».** Dans une bibliothèque de films, le titre en haut de la page est suivi du **nombre de films** (toutes sagas comprises ; il ne change pas quand vous affichez les sagas). En haut à droite, à gauche de l'heure, un petit interrupteur **Sagas** choisit l'affichage de l'onglet Bibliothèque : *désactivé* (par défaut), chaque film a sa propre affiche ; *activé*, les films d'une même saga sont regroupés derrière l'affiche de la saga, et **OK** dessus ouvre la saga et ses films. Votre choix est mémorisé. L'interrupteur n'apparaît que dans une bibliothèque de films, sur l'onglet Bibliothèque.

### Les films

Choisissez un film : sa **fiche** s'ouvre. En arrière-plan, la bande-annonce passe en silence et, si elle existe, une musique du film joue doucement.

Avant de lancer la lecture, vous pouvez régler directement sur la fiche :

- **Conv. forcée** (Oui / Non), à gauche de « Résolution » : demande au serveur de *convertir ce film* en entier au lieu de l'envoyer tel quel. À essayer si un film reste noir ou saccade alors que les autres passent. Le choix est mémorisé pour ce film seulement.
- **Résolution** : la qualité de l'image. Choisissez plus bas si la connexion est lente.
- **Audio** : la langue de la bande son.
- **Sous-titres** : une langue, ou « off ».

Les valeurs de départ viennent des paramètres. Appuyez sur **Lecture** (ou **Reprendre** si vous aviez commencé). À côté : **🎬 Trailer** lance la bande-annonce du film, et **Marquer lu** signale au serveur que vous l'avez déjà vu (un nouvel appui annule).

> Quand le serveur doit convertir le film (« Conv. forcée », changement de résolution, mode compatible, Box Player…), un message avec un indicateur tournant s'affiche avant la première image, par exemple « Création du cache et du transcodage, veuillez patienter… ». C'est normal : la lecture démarre ensuite.

### Les séries

- **La fiche de la série** : affiche, titre, années, nombre de saisons et d'épisodes, résumé, notes, et en dessous la rangée des saisons. **Lecture S2 E5** lance directement le prochain épisode à voir ; **🎬 Trailer** lance la bande-annonce de la série quand le serveur en connaît une (dans la langue proposée par le serveur Plex, parfois en anglais) ; **Marquer la série comme vue** coche tous les épisodes d'un coup (un second clic les décoche) ; le badge **« Reste 7 »** sur une saison indique le nombre d'épisodes qu'il vous reste à voir.
- **La page d'une saison** : tous ses épisodes en liste, avec vignette, numéro, titre, durée et résumé. Un épisode vu est marqué « Vu », un épisode commencé montre une barre de progression. La liste s'ouvre sur l'épisode en cours, ou le premier non vu.
- **Lancer un épisode** : sa page est identique à la fiche d'un film (résolution, audio, sous-titres, puis Lecture). Vos choix sont **mémorisés par série**. À la fin d'un épisode, le suivant démarre automatiquement (jusqu'à 5 de suite), avec les mêmes réglages audio et sous-titres.
- **Vu / non vu** : sur la page d'une saison, maintenez **OK** sur un épisode pour le marquer comme vu ou non vu. Sur une affiche de saison (fiche de la série), cela marque toute la saison.
- **Passer l'intro / le générique.** Quand votre serveur Plex a repéré l'intro d'un épisode (généralement avec un abonnement Plex Pass), un bouton **« Passer l'intro »** apparaît en bas de l'écran ; appuyez sur **OK** pour sauter directement à la suite. Même chose pour le générique de fin, avec **« Passer le générique »**, qui passe alors à l'épisode suivant. Deux réglages (voir plus bas) permettent de sauter l'intro et le générique **tout seul**, sans avoir à appuyer sur rien.

### Parcourir par style

Dans une bibliothèque de films ou de séries, l'onglet **Style** ouvre une fenêtre qui regroupe tous les genres : Humour, Action, Drame, Horreur, Science-fiction… **OK** sur le nom choisit le style, et la page montre tous les titres correspondants (le titre devient « Style : Humour », suivi du nombre de titres). Un titre qui a plusieurs genres apparaît dans chacun de ses styles. **Retour** ramène à la page normale de la bibliothèque.

### Idée TV : 5 films au hasard

Pas d'idée pour la soirée ? Dans une bibliothèque de films, le bouton **Idée TV** (tout à droite de la rangée d'onglets) propose **5 films tirés au hasard** parmi ceux que vous n'avez pas encore vus. Choisissez un thème dans le menu déroulant (ou « Pas de préférence »), découvrez les 5 affiches (chacune avec un bouton « Bande-annonce »), ouvrez-en une pour voir la fiche, ou demandez **Autre tirage** pour 5 nouveaux films.

### La recherche

Ouvrez **Recherche** dans le menu de gauche : un clavier s'affiche tout de suite. Déplacez-vous sur les lettres avec les flèches, **OK** pour taper. Dès 3 lettres, les résultats apparaissent (« mat » trouve « Matrix » ; accents et majuscules sont ignorés). Allez vers la droite pour choisir : les titres qui commencent par vos lettres viennent en premier. La recherche porte sur les bibliothèques affichées du serveur actif.

### Pendant la vidéo

| Touche | Effet |
|---|---|
| OK | Pause / lecture (sauf sur la barre de temps ou un bouton « Passer… », voir ci-dessous). |
| ← → | Reculer / avancer de 30 secondes dans la vidéo. |
| ▲ puis ← → | Sélectionne la barre de temps (elle grossit), puis déplace le curseur : 10 secondes par appui, 30 puis 60 secondes si vous maintenez la flèche. La lecture se déplace après un court instant, ou tout de suite avec OK. ▼ revient au bouton Lecture/Pause. |
| Retour | Quitter la lecture et revenir à la fiche. Votre progression est enregistrée : vous retrouvez le film dans « Continuer à voir ». |

La TV ne se met pas en veille pendant une vidéo.

**Le bouton « i »** de la barre de commandes :
- **Appui court** : la **fiche du titre en cours** — nom, année, durée, genres, public, note, réalisation, production, scénario, acteurs principaux, résumé, et une ligne « Lecture en cours » (résolution, format et langue du son, sous-titres), mise à jour en direct. Un nouvel appui court la referme.
- **Appui de 3 secondes** : les **données techniques** — 1ʳᵉ fois l'état de la lecture (lecture directe ou conversion par le serveur, décodeur de l'image et du son, images perdues, son reçu), 2ᵉ fois la page **Diagnostic** (appareil, écran, décodeurs de la TV, fichier d'origine, demande envoyée au serveur, réseau), 3ᵉ fois le panneau se ferme. Très utile si une vidéo pose problème : une photo de la page Diagnostic permet de comprendre rapidement ce qui se passe.

**Les prérolls avant le film.** Avant certains films, une courte annonce (un *préroll*) peut passer. Le réglage *Prérolls* choisit entre « Séquentiel externe » (un préroll différent à chaque film, dans l'ordre) et « Aléatoire serveur » (choisi par votre serveur Plex). Si un préroll ne peut pas être lu, un message « Erreur preroll » s'affiche brièvement et le film démarre normalement.

### Quitter et se déconnecter

- **Quitter Plexiplay** : depuis l'Accueil, appuyez sur **Retour**, puis choisissez *Oui* dans la fenêtre « Êtes-vous sûr ? ».
- **Se déconnecter** : dans les paramètres, ligne *Se déconnecter*, avec la même confirmation. Vous devrez ensuite ressaisir un code pour vous reconnecter.

## Les réglages

On y accède par la **roue crantée** en haut du menu de gauche. L'écran est présenté en plusieurs cadres : *Réglages principaux*, *Améliorations* (avec, pour les TV concernées, un sous-cadre *TV Philips et équivalent*), *Intros et génériques*, *Confort* et *Pratique*. Tout se commande à la télécommande :

- **▲ ▼** pour passer d'un réglage à l'autre ;
- **OK** sur un réglage pour changer sa valeur : à chaque appui, la valeur suivante s'affiche (la dernière revient à la première) ;
- pour les volumes, **OK** ouvre une liste : ▲ ▼ pour choisir, OK pour valider, Retour pour annuler ;
- **Retour** quitte les paramètres et revient à l'accueil.

Les changements sont enregistrés tout de suite, sans bouton « Valider ». À droite de chaque ligne, un petit texte gris rappelle en une phrase à quoi elle sert.

**Les manuels sont dans l'application.** En haut de la page, à droite du mot « Paramètres », deux petits boutons sous la mention *Manuels* ouvrent un guide sans quitter Plexiplay : **Utilisation** (le mode d'emploi) et **Réglages** (l'explication détaillée de chaque réglage). ▲ ▼ font défiler le texte, Retour le ferme.

Les valeurs d'origine conviennent à la grande majorité des installations : ne changez un réglage que si vous avez une raison précise.

| Réglage | Valeur conseillée | À changer seulement si… |
|---|---|---|
| **Réglages principaux** | | |
| Langue audio par défaut | fr | vous préférez la version originale |
| Sous-titres par défaut | off | vous voulez toujours des sous-titres |
| Lecteur | ExoPlayer | jamais, sauf TV très puissante de dernière génération |
| Puissance | TV | votre TV ou box est vraiment très ancienne (essayez alors SERVER) |
| Serveur | votre serveur habituel | vous avez plusieurs serveurs Plex |
| **Améliorations** | | |
| Bibliothèques affichées | celles que vous utilisez | le menu de gauche est trop chargé |
| Mode compatible | Automatique | une vidéo reste noire ou plante |
| Volume du son converti | Normal | le son est trop faible quand le serveur convertit le film |
| Box Player sur TV FullHD | Non | box d'opérateur sur TV Full HD, films 4K ou HDR noirs ou saccadés |
| Correction du format | Activée | l'image est déjà correcte et vous voyez un défaut |
| *TV Philips et équivalent* — Correctif Dolby Vision | Inactif | un film en Dolby Vision saute une image régulièrement, ou les annonces s'affichent mal après un tel film |
| **Intros et génériques** | | |
| Toujours passer les intros | Inactif | vous préférez sauter vous-même avec le bouton, plutôt que toute seule |
| Toujours passer les génériques | Inactif | idem, pour le passage automatique à l'épisode suivant |
| **Confort** | | |
| Thème | Classique | vous aimez les effets visuels (Néon, ou Futuriste sur une TV puissante) |
| Volume du générique | 40 % | la musique est trop forte, trop faible, ou vous n'en voulez pas |
| Prérolls | Séquentiel externe | vous préférez que le serveur Plex choisisse les annonces au hasard |
| Volume des prerolls | 75 % | les annonces sont trop fortes ou trop faibles |
| Désactivation des prerolls | non activée | vous voulez une pause des annonces pendant 7 jours |
| **Pratique** | | |
| Mises à jour | acceptez celles proposées | vous voulez vérifier à la main |
| Vérifier les invitations | – | on vous a invité sur un serveur ou ajouté en ami |
| Se déconnecter | – | vous changez de compte ou d'appareil |

Aucun réglage ne détruit quoi que ce soit : vous pouvez toujours revenir aux valeurs d'origine du tableau. Quelques précisions utiles :

- **Lecteur.** *ExoPlayer* est léger, fluide, pensé pour Android TV : c'est le bon choix dans presque tous les cas. *mpv* lit presque tout directement (DTS-HD, TrueHD, sous-titres PGS…) mais est beaucoup plus gourmand : il est réservé aux TV très puissantes et de toute dernière génération, et provoque des saccades en 4K sur les autres. La correction du format et le mode compatible ne s'appliquent pas à mpv.
- **Puissance.** *TV* : l'appli exploite d'abord ce que la TV sait faire (si elle ne décode pas un son DTS ou TrueHD, ExoPlayer le décode lui-même avec FFmpeg au lieu de le faire convertir par le serveur). *SERVER* : pensé pour décharger une TV peu puissante, avec un serveur costaud.
- **Mode compatible.** Certaines vidéos (souvent des films 4K en Dolby Vision avec une piste DTS-HD ou TrueHD) restent noires ou plantent sur certaines TV. Le mode compatible les rend lisibles : image en HDR10 au lieu de Dolby Vision, son converti par le serveur. En **Automatique**, si un film reste noir plus de 25 secondes, l'application le relance en mode compatible et s'en souvient pour ce film. *Activé* : tous les films, dès le début. *Désactivé* : jamais. Sous la ligne du réglage, « Codecs intégrés à la TV » indique ce que votre TV sait décoder. Concerne ExoPlayer uniquement.
- **Correctif Dolby Vision (TV Philips et équivalent).** Sur certaines TV, un film lu en Dolby Vision saute une image à intervalles réguliers, ou les prérolls qui suivent un tel film s'affichent zoomés, rayés ou teintés de violet jusqu'au redémarrage de la TV. En *Actif*, Plexiplay lit ces films avec le décodeur HEVC normal au lieu du décodeur Dolby Vision de la TV : l'image reste en 4K, le logo Dolby Vision s'affiche brièvement à chaque lancement, et les deux défauts disparaissent. Sans ce défaut, laissez ce réglage sur *Inactif*. Concerne ExoPlayer uniquement.
- **Box Player sur TV FullHD.** Pour une box d'opérateur branchée sur une TV Full HD : sur *Oui*, les films 4K, HDR ou 10 bits sont convertis par le serveur en image 1080p plus simple, ce qui règle les écrans noirs et les saccades.
- **Toujours passer les intros / les génériques.** Ces deux réglages dépendent de ce que votre serveur Plex a repéré sur chaque épisode (souvent avec un abonnement Plex Pass) : sans repère, ni bouton ni saut automatique n'apparaissent. En *Actif*, le saut se fait tout seul dès le début de l'intro ou du générique ; en *Inactif* (valeur d'origine), un bouton apparaît et c'est vous qui appuyez sur OK. Le saut automatique du générique ne s'applique qu'aux épisodes de séries, pour passer au suivant ; sur un film, seul le bouton existe.
- **Thème.** *Classique* (sobre), *Néon* (boutons en relief, couleurs vives), *Futuriste* (tous les effets du Néon plus un faisceau lumineux, des zooms, des transitions animées et des fiches en verre). Le Futuriste demande une TV ou un boîtier puissant : si l'affichage ralentit, revenez à Classique ou Néon, le changement est immédiat.
- **Prérolls.** *Séquentiel externe* : un seul préroll par film, dans l'ordre alphabétique des fichiers, puis retour au premier (demande un accès internet au lancement du film). *Aléatoire serveur* : les prérolls que votre serveur Plex choisit au hasard. Si le dossier des prérolls est introuvable, Plexiplay passe tout seul en « Aléatoire serveur » et la ligne du réglage est grisée.

## Un problème ? Quel réglage essayer

| Ce que vous constatez | Essayez |
|---|---|
| Un film reste noir ou plante au démarrage | **Mode compatible** sur Activé (ou laissez Automatique et patientez 25 s, il basculera seul) |
| Un film en Dolby Vision saute une image régulièrement | **Correctif Dolby Vision** sur Actif (cadre *TV Philips et équivalent*) |
| Après un film en Dolby Vision, les annonces suivantes s'affichent zoomées, rayées ou violettes | **Correctif Dolby Vision** sur Actif |
| Les visages sont étirés | **Correction du format** sur Activée ; vérifiez aussi le format d'image de la TV (pas de « 16/9 permanent ») |
| L'image saccade, surtout en 4K | **Lecteur** sur ExoPlayer (mpv n'est fait que pour les TV très puissantes et récentes) |
| Le son d'un film est absent ou étrange | **Mode compatible** sur Activé ; regardez la ligne « Codecs intégrés à la TV » sous le réglage |
| Je ne retrouve plus mes films | **Bibliothèques affichées** (une est peut-être masquée) et **Serveur** (est-ce le bon ?) |
| Une bibliothèque n'apparaît pas sur l'Accueil, alors qu'elle est dans le menu de gauche | Le serveur Plex ne l'autorise pas sur l'accueil (réglage Plex *Gérer les recommandations*) |
| Le son est trop faible quand le film est converti | **Volume du son converti** sur Renforcé ou Fort |
| Je veux savoir si le film est converti, et qui décode image et son | Bouton **« i »** de la barre de lecture, maintenu 3 secondes (un second appui long ouvre la page Diagnostic) |
| Écran noir ou saccades sur une box d'opérateur branchée à une TV Full HD, en 4K ou HDR | **Box Player sur TV FullHD** sur Oui |
| Un seul film reste noir ou saccade, les autres passent | Sur la fiche du film, **Conv. forcée : Oui** |
| Un message « Création du cache et du transcodage… » s'affiche | Rien à faire : le serveur prépare la conversion, la lecture démarre ensuite |
| Je veux que les annonces défilent dans l'ordre, ou au hasard | **Prérolls** : Séquentiel externe ou Aléatoire serveur |
| « Erreur preroll, merci de signaler… » apparaît | Notez le nom du fichier affiché et [signalez-le](#signaler-un-problème) ; le film démarre normalement |
| La ligne « Prérolls » est grisée | Normal : le dossier des prérolls est introuvable, les prérolls du serveur Plex sont utilisés |
| La musique des séries est trop forte | **Volume du générique** à 10 % ou 0 % |
| Les annonces avant le film sont trop fortes | **Volume des prerolls** plus bas (50 % ou moins) |
| Je ne veux plus d'annonces pendant un moment | **Désactivation des prerolls** (pause de 7 jours, annulable) |
| Je veux sauter l'intro ou le générique sans appuyer sur rien | **Toujours passer les intros** / **Toujours passer les génériques** sur Actif |
| Le défilement n'est pas fluide avec le thème Néon ou Futuriste | **Thème** sur Classique |
| On m'a invité sur un serveur | **Vérifier les invitations**, puis le réglage **Serveur** |
| Je veux la dernière version tout de suite | **Mises à jour** : « Recherche mise à jour », puis « Mise à jour » |
| L'application me redemande un code de connexion | Normal après un certain temps, ou si vous avez retiré l'appareil depuis votre compte plex.tv : refaites simplement un code |

## Questions fréquentes

**Je ne vois pas mes films / « serveur injoignable ».** Vérifiez dans les paramètres la ligne *Serveur* (si vous avez plusieurs serveurs, appuyez dessus pour passer à un autre) et *Bibliothèques affichées* (elles sont peut-être décochées). Si un écran explique que le chargement a échoué, choisissez **Réessayer**, ou **Se reconnecter** si le problème persiste.

**La vidéo saccade ou ne démarre pas.** Choisissez une résolution plus basse sur la fiche. Dans les paramètres, essayez *Puissance : SERVER* et le lecteur *ExoPlayer*. Si un film ne démarre pas du tout, essayez *mpv*.

**Je ne trouve pas de sous-titres.** Le film ne les contient peut-être pas. Sur la fiche, la ligne *Sous-titres* liste uniquement ce qui existe pour ce film.

**Écran noir ou saccades avec une box d'opérateur.** Si la box est branchée sur une TV Full HD, activez *Box Player sur TV FullHD*. Si un seul film pose problème, mettez *Conv. forcée* sur Oui sur sa fiche. Pour comprendre la cause, maintenez « i » 3 secondes pendant la lecture, deux fois de suite.

**Le thème Futuriste ralentit l'affichage.** Il demande une TV ou un boîtier puissant et récent : repassez sur *Néon* ou *Classique*.

**Comment mettre à jour ?** Paramètres, ligne *Recherche mise à jour* : appuyez dessus, puis choisissez *Mise à jour* si une version est proposée. L'application vérifie aussi seule à chaque démarrage.

**Comment retirer un titre de « Continuer à regarder » ?** Maintenez OK 3 secondes sur l'affiche, puis choisissez *Supprimer de « Continuer à regarder »*.

**Comment avancer ou reculer précisément dans une vidéo ?** Depuis un bouton de la barre de lecture, appuyez sur ▲ pour sélectionner la barre de temps, puis ← → pour déplacer le curseur.

**Comment sauter l'intro ou le générique sans y penser ?** Activez *Toujours passer les intros* et *Toujours passer les génériques* dans les paramètres. Cela ne fonctionne que si votre serveur Plex a repéré ces passages.

**Puis-je regarder le serveur d'un ami ?** Oui, à condition qu'il l'ait partagé avec votre compte Plex. Il apparaît alors dans la ligne *Serveur* des paramètres.

## Ce qui viendra plus tard

Plexiplay évolue régulièrement. Certaines fonctions ne sont pas encore disponibles :

- la **reprise à la position exacte** d'un épisode de série commencé ;
- un **compte à rebours** avant le lancement automatique de l'épisode suivant ;
- le **changement de profil** Plex Home directement depuis l'application ;
- d'autres fonctions secondaires, au fil des mises à jour.

Chaque nouvelle version est publiée dans les [Releases](https://github.com/Kahenis/plexiplay/releases) et se télécharge ensuite depuis les paramètres de Plexiplay : rien d'autre à installer.

## Signaler un problème

Une vidéo ne se lit pas, un message d'erreur apparaît, une idée d'amélioration ? Ouvrez un [ticket](https://github.com/Kahenis/plexiplay/issues/new) en indiquant la marque et le modèle de votre TV ou box, la version de Plexiplay (visible dans *Paramètres → Mises à jour*) et, si une vidéo pose problème, une photo de la page **Diagnostic** (bouton « i », maintenu 3 secondes deux fois de suite pendant la lecture).

---

Plexiplay · conçu et développé par Jean-Francois Guilard.
