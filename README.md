# ACC 9000 — coach de progression Assetto Corsa Competizione

Site : https://victorhaegeman.github.io/acc-9000/

Un coach qui te dit quoi rouler pour faire monter tes ratings ACC, et qui s'adapte après chaque session.

## Comment ça marche

1. **Démarrer** : l'app te propose 3 sessions recommandées, calculées sur tes points faibles (Safety, Pace, médailles…). Chaque carte indique ce qu'elle fait progresser. Tu peux aussi lancer une session personnalisée.
2. **Rouler** : chrono, consignes à cocher, compteurs de contacts et de sorties de piste. Tout est sauvegardé en continu, tu peux fermer l'onglet pendant que tu roules.
3. **Terminer** : tu entres ta Safety après la session (et tous tes ratings si tu veux). L'app apprend quels types de sessions te font progresser et ajuste ses recommandations.

Pages : Accueil, Session, Objectifs (hebdo), Progression (graphiques), Historique, Médailles, Guide, Réglages.

## Objectif : la compétition

La page **Compétition** suit la feuille de route vers les vraies courses en ligne : 80 de Safety, test de licence LFM, première course LFM, licences Iron, Bronze et Silver (Elo, nombre de courses, safety LFM), premier championnat, équipe. Les phases, les sessions recommandées et les objectifs suivent cette feuille de route. Le Total ACC reste affiché en bonus : il ne donne aucun accès.

## Ce qui s'adapte à toi

- **Temps dispo** (20 min, 45 min, 1 h 30) : les sessions trop longues passent en bas et la course IA est raccourcie.
- **Variété** : une session déjà faite aujourd'hui descend dans les recommandations.
- **Causes de contact** : pendant une course, tu touches la situation de chaque contact (départ, dépassement, défense, subi). Si une cause domine, elle devient la première consigne de tes courses, un objectif de la semaine, et elle ajuste la grille et l'IA.
- **Objectifs automatiques** : ils avancent tout seuls avec les sessions enregistrées (barre de progression), sauf les règles du type « pas de serveur ouvert », vérifiées sur la semaine.
- **Passage de phase** : annoncé à la fin de la session qui le déclenche.
- **Pistes non possédées** (DLC) : « Je ne l'ai pas » dans Médailles ou sur la page Préparer, elles ne sont plus jamais recommandées.

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
