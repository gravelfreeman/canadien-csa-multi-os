> Attention : dans ce guide, je fais souvent référence à la touche `ù Ù`, absente de Windows et Linux. Elle existe bien sur les claviers ISO, à gauche de `Shift`, mais ce guide est basé sur un clavier US, le plus répandu. Dans ce contexte, cette touche n’existe donc pas. Si vous utilisez un clavier ISO international, ce guide ne s’appliquera pas entièrement.

<img width="2000" height="711" alt="image" src="https://github.com/user-attachments/assets/00ce1358-6a72-426c-bd1d-244e7545017e" />

***

[Introduction](#introduction)  

[1. Hardware](#1-hardware)  
- [1.1 Clavier mécanique](#11-clavier-mécanique)  
- [1.2 Touches Canadien-CSA](#12-touches-canadien-csa)  

[2. Software](software)  
- [2.1 Configuration du clavier](#21-configuration-du-clavier)  
- [2.2 Canadien - CSA (Alt)](#22-canadien---csa-alt)  
- [2.3 Mapping des touches](#23-mapping-des-touches)  

[Conclusion](conclusion)

# Introduction

Depuis des années je jongle entre Windows, macOS et Linux. Entre les partisans du Canadien-CSA (accents sans touche morte) et ceux qui préfèrent le Français Canada, rien n’est simple. Selon moi, Français Canada est un mauvais compromis : trop de touches manquantes, des caractères essentiels trop éloignés, et un décalage complet dès qu’on utilise un clavier Mac, où seule la sérigraphie CSA existe.

Jusqu’ici je survivais grâce à la mémoire musculaire. J’en ai eu assez : je voulais un moyen propre, cohérent et stable pour passer d’un OS à l’autre sans perdre mes repères. La documentation est rare. Je m’y attelle parce que personne ne semble vouloir le faire. Le sujet est complexe : pour un vrai résultat, il faut intervenir à la fois au niveau matériel et logiciel, ce qui rend difficile toute solution monétisable ou “officielle”.

Voici donc ma méthode, assumée et perfectible. Adaptez-la à votre goût. Si vous suivez mon approche, vous aurez un clavier fonctionnel en français, en anglais et pour la programmation.

> J’ai volontairement exclu les caractères avancés de rédaction et de science : Windows ne les gère pas nativement et leur présence surcharge inutilement un clavier dont on n’a pas besoin 99 % du temps.

# 1. Hardware

## 1.1 Clavier mécanique

J’utilise un **MCHOSE GX87 Ultra**, disponible chez [beaverkeys](https://beaverkeys.ca/products/mchose-gx87-ultra)

Boutique fiable, commandes multiples, envois rapides et service impeccable. Pour moi, c’est le meilleur rapport qualité-prix : la qualité est identique au clavier custom d’un ami qui lui a coûté près de 800 $. Donc non, ce n’est pas cher. Je suis du genre r/buyitforlife ce clavier est entièrement réparable et tiendra une vie.

Il passe parfaitement de la programmation au gaming sans que j’aie à changer de setup. Je dois déjà alterner entre une MX Master et une G Pro en gaming, alors multiplier les périphériques serait infernal. J’aimais les claviers avec pavé numérique, mais en gaming ça gêne trop la souris. Depuis que je suis passé à un format compact, je ne reviendrais plus en arrière, c’est bien plus ergonomique et ça recentre naturellement la position de travail.

## 1.2 Touches Canadien-CSA

J’ai créé un [template Canadien-CSA](https://yuzukeycaps.com/c/311360fd-f41f-43e8-b996-5f66f2d66d6a) avec **YUZU Custom Keycaps** pour 95 USD shipping inclus.

C’est cher, mais normal pour du custom sans group buy.

Pour y parvenir, j’ai comparé les layouts Windows, macOS et Linux — Canadien multilingue, Canadien-CSA et Canadien Intl. — afin d’identifier ce qui se recoupe et ce qui diverge. Le résultat implique forcément des compromis que j’explique ici.

1. Sur Mac, la touche à gauche du 1 donne `ù Ù`. Elle n’existe pas sur Windows et Linux, qui utilisent plutôt `/ \ |`. Perdre cette touche me dérangeait, elle est trop utile en programmation. Je l’ai donc réaffectée à `/ \ |` via un profil personnalisé fourni dans le repo.

2. Sur Mac, la touche `Commande` est inversée avec la touche `Win`. C’est pourquoi les touches `Commande`|`Win` et `Option`|`Alt` ne se retrouvent pas sur la même touche à gauche de la barre d’espacement. Il serait impossible sur Mac de faire un Alt-Tab ou d’utiliser les raccourcis comme le presse-papier avec la touche `Alt` d’un clavier standard.

<img width="485" height="56" alt="image" src="https://github.com/user-attachments/assets/26a3f6b6-29a5-4d1a-a42b-8696f84ddbc4" />

3. Au contraire, à droite de la barre d’espacement, vous trouverez les combinaisons `Option + Alt` et `Commande + Win`.

La raison est simple :
* sur Windows, le layer 2 s’active avec `AltGr`
* sur Mac, il s’active avec Option, située une touche plus à droite de `AltGr`

Si je ne réorganisais pas ces touches, il faudrait utiliser un bouton différent pour accéder au layer 2 selon l’OS. Avec cette disposition, la même touche sert pour Windows, Linux et macOS, ce qui évite de casser la mémoire musculaire.

<img width="486" height="57" alt="image" src="https://github.com/user-attachments/assets/c866271f-35b7-4a7a-98dc-650204c0767c" />

# 2. Software

## 2.1 Configuration du clavier

Configurer chaque OS avec les modèles de clavier suivants :

| OS  | Clavier |
| ------------- | ------------- |
| Windows | Canadien multilingue standard  |
| MacOS | Canadien - CSA (Alt) |
| Linux | Canadien Intl. |

## 2.2 Canadien - CSA (Alt)

Tel qu'expliqué ci-haut, sur Mac, la touche à gauche du 1 donne `ù Ù`. Elle n’existe pas sur Windows et Linux, qui utilisent plutôt `/ \ |`. Je l’ai donc réaffectée à `/ \ |` via un profil alternatif appelé `Canadien - CSA (Alt)` fourni dans le repo.

> Note: Igorez cette étape si vous désirez conserver la touche `ù Ù` sur Mac même si elle diffèrera de la touche Windows et Linux.

Une fois le dossier *Canadien - CSA (Alt)* téléchargé à partir du repo, copier le tout simplement dans le dossier suivant :

```
~/Library/Keyboard Layouts
```

Il devrait maintenant être disponible dans les paramêtres Claviers de votre Mac.

## 2.3 Mapping des touches

Tel qu'expliqué ci-haut sur Mac, la touche `Commande` est inversée avec la touche `Win`. Il serait impossible sur Mac de faire un Alt-Tab ou d’utiliser les raccourcis comme le presse-papier avec la touche `Alt` d’un clavier standard. Nous allons remapper ces touches afin que cela fonctionne.

Pour ce faire, je n’utilise pas l’option native de macOS, car elle ne permet pas de modifier uniquement les touches situées à gauche de la barre d’espacement (voir Hardware/Touches Canadien-CSA plus haut). Il faut donc passer par le Terminal et appliquer la réaffectation manuellement. Une application comme Karabiner peut faire l’équivalent, mais je trouve que c’est trop d'overhead pour deux simples remappages. Je préfère une solution plus propre et minimale.

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

Facultatif, désinstaller au besoin :

```
hidutil property --set '{"UserKeyMapping":[]}'
```

# Conclusion

C’est la méthode la plus rapide que j’ai trouvée pour basculer avec un KVM. Elle évite d’avoir à passer du mode Mac au mode Windows sur le clavier, avec des mappings différents selon l’OS, ou à gérer plusieurs layers dans VIA. Sur le GX87, maintenir Fn + A après un switch KVM est beaucoup trop lent. Je voulais une configuration set and forget : quelque chose qui survive aux mises à jour système et qui ne dépende d’aucune application tierce. C’est léger, transparent et, une fois configuré, on n’y touche plus. J’espère que mon casse-tête servira à d’autres; si vous avez des suggestions, n’hésitez pas à ouvrir un issue sur le GitHub. Pour ajouter des modèles de claviers, vous pouvez faire une PR et je regarderai ça.
