FICHIERS INCLUS
- index.html : contient le correctif du menu références (datalist) + boutons NEUF/USITÉ exclusifs
- sw.js : correctif PWA (network-first sur les pages) + cache versionné
- manifest.json : manifest PWA minimal
- icon-192.png / icon-512.png : icônes de base

IMPORTANT (Android / PWA)
Si tu avais déjà installé l'appli (PWA) ou si tu avais un cache, fais ça après avoir remplacé les fichiers :
1) Désinstalle l'appli PWA (si installée)
2) Chrome > Paramètres du site > Stockage > Effacer (pour ton domaine)
3) Recharge la page, puis réinstalle

REFERENCES (menu)
Ce correctif lit une liste optionnelle dans localStorage sous la clé:
  REFERENCES_LIST
Formats acceptés :
  ["REF-001","REF-002"]
ou
  [{"value":"REF-001","label":"REF-001 - Détecteur PIR"}, ...]

CACHE PWA
Si tu modifies à nouveau, change la ligne dans sw.js :
  const CACHE_NAME = "inventaire-pwa-vX-....";

Généré le 2026-01-30.
