# ACC 9000 — coach de progression Assetto Corsa Competizione

Site : https://victorhaegeman.github.io/acc-9000/

Un coach qui te dit quoi rouler pour faire monter tes ratings ACC, et qui s'adapte après chaque session.

## Comment ça marche

1. **Démarrer** : l'app te propose 3 sessions recommandées, calculées sur tes points faibles (Safety, Pace, médailles…). Chaque carte indique ce qu'elle fait progresser. Tu peux aussi lancer une session personnalisée.
2. **Rouler** : chrono, consignes à cocher, compteurs de contacts et de sorties de piste. Tout est sauvegardé en continu, tu peux fermer l'onglet pendant que tu roules.
3. **Terminer** : tu entres ta Safety après la session (et tous tes ratings si tu veux). L'app apprend quels types de sessions te font progresser et ajuste ses recommandations.

Pages : Accueil, Session, Objectifs (hebdo), Progression (graphiques), Historique, Médailles, Guide, Réglages.

## Sauvegarde automatique

À choisir dans **Réglages** :

- **GitHub (recommandé)** : tes données sont écrites automatiquement dans un dépôt privé, par exemple `acc-9000-data`, fichier `data/<ton-pseudo>.json`. Tu les retrouves sur n'importe quel appareil.
  1. Crée un dépôt **privé** `acc-9000-data` (coche « Add a README »).
  2. GitHub → Settings → Developer settings → Personal access tokens → **Fine-grained tokens** → Generate new token.
  3. Repository access : **Only select repositories** → `acc-9000-data`. Permissions : **Contents : Read and write**.
  4. Colle le token dans Réglages → Sauvegarde GitHub.

  Le token reste uniquement dans ton navigateur. Il n'est jamais écrit dans tes données ni sur GitHub.
- **Fichier sur ton PC** (Chrome et Edge) : un fichier `.json` mis à jour à chaque modification. Mets-le dans OneDrive ou Google Drive pour l'avoir partout. Brave et Firefox bloquent cette option par défaut.
- **Export / import** manuel en secours.

## Partager avec un pote

Il ouvre le même lien et crée son profil avec ses propres stats. Ses recommandations et objectifs sont calculés sur ses points faibles. Pour sa sauvegarde : son propre dépôt, ou ajoute-le en collaborateur sur `acc-9000-data` et il utilise son fichier (`data/son-pseudo.json`) avec son propre token.
