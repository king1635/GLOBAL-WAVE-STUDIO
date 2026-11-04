# GLOBAL WAVE STUDIO — première étape d'identité

## Base technique
GLOBAL WAVE STUDIO est une distribution/fork de LYNX-SHARE. Le moteur audio, le séquenceur, le navigateur, le piano roll, la playlist, le mixer et les formats de projet restent ceux du projet amont tant qu'ils n'ont pas été explicitement modifiés et testés.

## Direction visuelle
- Fond principal : `#171A20`
- Accent de marque : cuivre/orange `#E89A3C`
- Texte principal : `#ECEEF2`
- Texte secondaire : `#A1A6B0`
- Surfaces en élévation : nuances anthracite
- Vert : état audio actif / LED
- Rouge : enregistrement, clipping et alertes critiques
- Cyan : automation
- Bleu : informations secondaires

## Principes d'implémentation
1. Garder les changements de palette centralisés dans `src/ui/Theme.h` et `src/core/ThemePalette.*`.
2. Préserver les couleurs sémantiques qui ne sont pas l'accent de marque.
3. Ne pas modifier le chemin audio temps réel pour un changement graphique.
4. Préserver les extensions, formats et chemins d'installation amont jusqu'à ce qu'une migration dédiée et testée soit livrée.
5. Toute évolution UI doit être testée sur Windows 11 et, lorsque possible, macOS et Linux.

## Compatibilité et licence
Le dépôt dérive de LYNX-SHARE et conserve sa licence GNU AGPL-3.0. Consulter `LICENSE` et `THIRD_PARTY.md` avant toute distribution. Les marques et noms de plugins tiers ne sont pas des actifs de GLOBAL WAVE STUDIO.
