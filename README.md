> Attention : Ce guide s'addresse aux utilisateurs désirant configurer leur clavier suivant la norme [CAN/CSA Z243.200](https://fr.wikipedia.org/wiki/CAN/CSA_Z243.200) niveau A, également connu sous le nom de *Canadien - CSA* sur *macOS*, *Canadien multilingue* sur *Windows* et *Canadien Intl.* sur *Linux*.

<img width="2000" height="822" alt="Canadien - CSA(4)" src="https://github.com/user-attachments/assets/5586e630-37e2-4766-bf7b-b4da62561c4c" />

***

# Introduction

Depuis des années je jongle entre Windows, macOS et Linux et j'ai créé un modèle de *Keycaps* universel s'adaptant d'un OS en utilisant le minimum de modification au niveau des différents système d'exploitation. Adaptez à votre goût selon vos besoins comme chacune des parties de ce guide son facultatives.

Si vous suivez mon approche, vous aurez un clavier fonctionnel en français, en anglais et pour la programmation affichant les bons glyphes sur chacune des touches de votre clavier physique, respectant ainsi la norme [CAN/CSA Z243.200](https://fr.wikipedia.org/wiki/CAN/CSA_Z243.200) niveau A, populaire notamment sur les claviers de marque Apple.

[1. Modèle CAN/CSA Z243.200](#1-modèle-cancsa-z243200)  
- [1.1 Sélection du format](#11-sélection-du-format)  
- [1.2 Personnalisation](#12-personnalisation)

[2. Configuration](#2-configuration)  
- [2.1 Configuration du clavier](#21-configuration-du-clavier)  
- [2.2 Configuration ANSI (É.-U.)](#22-configuration-ansi-é-u)
- [2.3 Configuration macOS](#23-configuration-macos)
- [2.3.1 Mapping de base](#231-mapping-de-base)
- [2.3.2 Mapping avancé](#232-mapping-avancé)

# Compatibilité

Ce guide est compatible avec les claviers *ANSI (É.-U.)* et *ISO (international)*.

| Type | Formats | Touches |
|------|---------|----------|
| ANSI&nbsp;(É.-U.)<br>ISO&nbsp;(international) | Full Size, TKL, 75%, 65%, 60%, 40%, Ortho, Alice, Corne, Split 3×5, Lily 58, Sofle, 1800, Ergolite, HHKB | ISO Enter, Split Left Shift, Tsangan/WKL, Stepped Caps Lock, Split Backspace, Split Right Shift, F13, Split Numpad Plus, Split Numpad Enter, Split Numpad Zero, Split Spacebar, 4× R1, 6.25u Spacebar |

Ainsi que tout autre format ou touche personnalisée avec un minimum d’efforts.

# 1. Modèle CAN/CSA Z243.200

J’ai créé un modèle universel et personnalisable [CAN/CSA Z243.200](https://fr.wikipedia.org/wiki/CAN/CSA_Z243.200) niveau A, avec **YUZU Custom Keycaps**. Selon le format de votre clavier, et donc le nombre de touches, le coût devrait tourner autour de **$100 USD, expédition incluse**.

Cette option peut paraître coûteuse si vous n’utilisez pas souvent votre clavier, et vous préférerez peut-être conserver vos touches actuelles ou fabriquer les vôtres. Dans tous les cas, n’hésitez pas à passer à l’étape suivante si les symboles imprimés sur les touches ne sont pas essentiels pour vous.

Lien vers le modèle : https://yuzukeycaps.com/c/e71fa997-c839-47f1-8e26-ca5547bbc25a

> Note : Par souci de transparence, si vous achetez mon modèle ou passez par ce lien, je recevrai une petite commission, ce qui est grandement apprécié pour le temps investi.

## 1.1 Sélection du format

Sur la page d’édition, cliquez simplement sur *Rechercher* dans l’onglet *Paramètres*.

<img width="404" height="227" alt="image" src="https://github.com/user-attachments/assets/369f97bd-671f-4ca5-8efe-70ab2fc6b97f" />

Vous pourrez alors choisir le format ainsi que votre modèle de clavier actuel, ou un équivalent.

## 1.2 Personnalisation

Si vous le souhaitez, vous pouvez modifier les couleurs à votre convenance en ouvrant l’onglet *Couleurs* puis en sélectionnant celles que vous voulez changer.

<img width="416" height="468" alt="image" src="https://github.com/user-attachments/assets/b1b2dcaf-0b7b-4908-bf09-20705df53e4f" />

Si vous souhaitez conserver le code de couleur et uniquement ajuster les teintes, voici quelques informations utiles :

GR2 : Couleur de `touche` principale et `icône`<br>
GR5 : Couleur de `touche` secondaire<br>
GR13 : Couleur de `caractère` principale et `caractère` secondaire (shift)<br>
GN3 : Couleur de `caractère` tier (alt) et `échap`<br>
GN28+GN27+GN26 : Dégradé de couleur pour `touche` tierce<br>

***

Vous pouvez également personnaliser la police d’écriture dans l’onglet *Légendes*. La police par défaut est **Nunito**.

Voici un exemple avec des couleurs personnalisées :

<img width="2034" height="892" alt="image" src="https://github.com/user-attachments/assets/0d819aa4-5cec-4aca-b4bc-0d845bc1f085" />
<br>
> Note : Vous pouvez bien sûr tout modifier comme bon vous semble à l’aide de cet outil, mais cela dépasse le cadre de ce guide.

# 2. Configuration

## 2.1 Configuration du clavier

Configurer chaque OS avec les modèles de clavier suivants :

| OS  | Clavier |
| ------------- | ------------- |
| Windows | Canadien multilingue standard  |
| MacOS | Canadien - CSA/Alt |
| Linux | Canadien Intl. |

## 2.2 Configuration ANSI (É.-U.)

> Si vous possédez un clavier de type *ISO (international)*, le contenu de cette section ne s’applique pas à vous.

Pour les utilisateurs d’un clavier de type `ANSI (É.-U.)`, vous constaterez que *macOS* réaffecte automatiquement la touche `ù Ù` à la place de la touche `/ \ |`, normalement située à gauche du `1`.
Sur un clavier *ISO (international)*, la touche `ù` se trouve à droite de `Shift` (gauche).

Par souci de cohérence avec *Windows* et *Linux* — sachant qu’il est possible de produire le caractère `ù` avec `Alt` + `^` + `u` — j’ai réaffecté la touche `/ \ |` à sa place d’origine au moyen d’un profil de clavier personnalisé **Canadien – Alt**, disponible dans le dépôt.

> Note : Ignorez cette étape si vous désirez conserver la touche `ù Ù` sur *macOS* même si elle diffèrera sur *Windows* et *Linux*.

Une fois le dossier *Canadien - Alt* téléchargé à partir du repo, copier le tout simplement dans le dossier suivant :

```
~/Library/Keyboard Layouts
```

Il devrait maintenant être disponible dans les paramêtres *Claviers* de votre Mac.

## 2.3 Configuration macOS

Sur *macOS*, la touche `Commande` est inversée avec la touche `Win`. C’est pourquoi les touches `Commande`|`Win` et `Option`|`Alt` ne se trouvent pas sur la même touche.

Cela correspond au remappage de base décrit en *2.3.1*.

<img width="140" height="57" alt="image" src="https://github.com/user-attachments/assets/d18dbda6-7d88-4aac-b24c-3cf03c4b6cf8" />

***

À droite de la barre d’espacement, vous remarquerez toutefois une différence majeure entre macOS et Windows :

* sous *Windows*, le niveau 3 s’active avec `AltGr`
* sous *macOS*, il s’active avec `Option`, placée une touche plus à droite que `AltGr`

Il faut donc utiliser une touche différente pour accéder au niveau 3 selon l’OS.

Si vous souhaitez harmoniser cette disposition, privilégiez la méthode avancée décrite en *2.3.2*, afin qu’une seule et même touche active le niveau 3 sur *Windows*, *Linux* et *macOS*.

D’ailleurs, le modèle personnalisé disponible sur *YUZU* inclut deux touches additionnelles, `Option + Alt` et `Commande + Win`, prévues précisément pour cet usage.

<img width="486" height="57" alt="image" src="https://github.com/user-attachments/assets/c866271f-35b7-4a7a-98dc-650204c0767c" />

***

### 2.3.1 Mapping de base

> Note : Ignorer si vous avez utilisé la méthode avancée de *2.3.2*.

1. Ouvrir les réglages système et sous l'onglet `Clavier`, cliquez sur `Raccourcis clavier...`

2. Dans la fenêtre qui vient de s'ouvrir, cliquez sur l'onglet `Combinaison de touches` et interchanger les touches `Commande` et `Option` :

<img width="472" height="438" alt="image" src="https://github.com/user-attachments/assets/da1aae21-d640-452a-a8b1-c686e8dbc34e" />

### 2.3.2 Mapping avancé

> Note : Ignorer si vous avez utilisé la méthode avancée de *2.3.1*.

Pour ce faire, je n’utilise pas l’option native de macOS, car elle ne permet pas de modifier uniquement les touches situées à gauche de la barre d’espacement. Il faut donc passer par le Terminal et appliquer la réaffectation manuellement. Une application comme Karabiner peut faire l’équivalent, mais je trouve que c’est trop d'overhead pour un simple remappage.

1. Dans un terminal, créer le fichier `com.custom.hidutil.plist` avec cette commande :

```
sudo nano /Library/LaunchDaemons/com.custom.hidutil.plist
```

```xml
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE plist PUBLIC "-//Apple//DTD PLIST 1.0//EN" "http://www.apple.com/DTDs/PropertyList-1.0.dtd">
<plist version="1.0">
<dict>
  <key>Label</key>
  <string>com.custom.hidutil</string>
  <key>ProgramArguments</key>
  <array>
    <string>/usr/bin/hidutil</string>
    <string>property</string>
    <string>--set</string>
    <string>{"UserKeyMapping":[{"HIDKeyboardModifierMappingSrc":0x7000000E2,"HIDKeyboardModifierMappingDst":0x7000000E3},{"HIDKeyboardModifierMappingSrc":0x7000000E3,"HIDKeyboardModifierMappingDst":0x7000000E2}]}</string>
  </array>
  <key>RunAtLoad</key>
  <true/>
</dict>
</plist>
```

2. Puis charge-le :

```
sudo launchctl load /Library/LaunchDaemons/com.custom.hidutil.plist
```

Désinstallation au besoin :

```
hidutil property --set '{"UserKeyMapping":[]}'
```
