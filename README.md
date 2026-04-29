# 🌊 Biodiversité Marine – VR Quest

Expérience de réalité virtuelle WebXR immersive sur la biodiversité marine, compatible **Meta Quest** et tout navigateur supportant WebXR (Chrome, Edge, Firefox Reality).

## ✨ Fonctionnalités

- 🌊 **Monde sous-marin** complet : fond marin, coraux, algues, rayons de lumière (caustiques), bulles remontantes et plancton
- 🐾 **7 espèces animées** :
  - 🐬 Grand Dauphin × 3 (nage en orbite, nageoire caudale animée)
  - 🐋 Baleine à Bosse (grande envergure, longues nageoires pectorales)
  - 🦈 Grand Requin Blanc (nage en profondeur)
  - 🐢 Tortue Verte (nageoires battantes)
  - 🐙 Pieuvre (tentacules ondulants)
  - 🐠 Poissons Clown × banc de 5 (autour d'une anémone animée)
  - 🦩 Raie Manta (vol plané en figure 8, ailes battantes)
  - 🪼 Méduses × 2 (pulsation translucide)
- 📋 **Fiche explicative** pour chaque animal : regardez-le 1,5 s (fuse cursor) ou cliquez pour lire
- 🗂️ **Panneau légende** flottant dans la scène

## 🚀 Démarrage rapide

```bash
# Option 1 – ouvrir directement (Chrome / Edge)
open index.html

# Option 2 – serveur local (recommandé pour WebXR)
npx serve .
# puis naviguer sur http://localhost:3000
```

> **Meta Quest** : activez le mode développeur, ouvrez l'URL dans le navigateur Quest, appuyez sur **Entrer en VR**.

## 🎮 Contrôles

| Action | Résultat |
|--------|----------|
| Regarder un animal ≥ 1,5 s | Affiche la fiche (desktop / regard) |
| Clic / trigger | Affiche la fiche instantanément |
| WASD + souris | Déplacement libre (desktop) |
| Manettes Quest | Locomotion WebXR standard |

## 🛠️ Technologies

- [A-Frame 1.5](https://aframe.io/) – WebXR framework
- Géométries A-Frame personnalisées (ellipsoïde)
- Composants custom : `swim`, `tail-wag`, `bubble-rise`, `jelly-pulse`, `ray-glide`, `animal-info`
- Zéro dépendance externe côté serveur – fichier HTML unique