# Joyeuse - Conteuse Merveilleuse

## Appareil
- **Produit** : La Conteuse Merveilleuse (cube à histoires pour enfants 0-6 ans)
- **Marque** : Joyeuse (joyeuse.io), fabriqué en France
- **Modèle** : CUBE
- **Firmware** : V05.15
- **S/N** : JOY_3D00400010PHPN69X_1
- **Stockage** : 125,5 Mo, FAT, label JOYEUSE-515
- **Montage USB** : `/media/alexis/JOYEUSE-515`

## Fonctionnement
- Cube avec 6 faces, chaque face = une catégorie de contenu audio (MP3)
- Interaction par gestes : secouer, taper, retourner
- Se monte comme une clé USB pour gérer le contenu (glisser-déposer MP3)
- Paramétrage parental via `Secrets/SETTINGS.txt` (volume, mode nuit, sensibilité, etc.)

## Structure sur le cube
```
/media/alexis/JOYEUSE-515/
├── FR/
│   ├── ABCDAIRE/     # Fables de La Fontaine (7 MP3)
│   ├── COEUR/        # Histoires préférées (auto/manuel)
│   ├── JAUNE/        # Comptines (5 MP3, préfixe @07-@11)
│   ├── LION/         # Contes classiques (16 MP3)
│   ├── NUAGE/        # Histoires du soir / Noël (5 MP3)
│   └── ROUGE/        # Histoires rigolotes (12 MP3)
├── Secrets/          # Config système, sons système, settings
├── bonjour.txt       # Message de bienvenue parents
└── autorun.inf
```

- Chaque face peut avoir un sous-dossier `_hors liste de lecture/` pour du contenu exclu
- Préfixer les fichiers `@NN_` ou `_NN_` pour forcer l'ordre de lecture

## Bibliothèque en ligne
- **Fichier** : `library.csv` (234 produits, scrapé le 2026-03-08)
- **Source** : https://www.joyeuse.io/collections/library (filtre: Français)
- **Prix** : 0,99€ à 19,99€ (moyenne ~9€)
- **Éditeurs principaux** : Didier Jeunesse (69), Victorie Music (58), Joyeuse (36), Henri Dès/PMJ (20), Trois Petits Points (19)
- **Contenu** : histoires, comptines, chansons, berceuses, balades sonores, contes musicaux

## Site & Support
- Site : https://www.joyeuse.io
- Contact : club@joyeuse.io
- La Moulinette (sur le site) : convertisseur MP3/CD au format Joyeuse
- Studio : enregistrement d'histoires personnelles
