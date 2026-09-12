# WebCRM — Fiche de situation bénéficiaire / Beneficiary status sheet

Application web **100 % locale** (un seul fichier `index.html`, aucune dépendance, aucune donnée
envoyée sur Internet) permettant de produire une **situation sur un client / bénéficiaire d'un
programme financier**, avec **rendu bilingue Français / Anglais** et **export PDF téléchargeable**.

---

## 🎨 Design du document / Document design

Rendu type **fiche de Cabinet / banque** : en-tête à papier (logo, filet double marine & or),
titre serif lettré, **bandeau des chiffres clés** (montant sollicité · mensualité · forfait assurance),
sections numérotées **01 → 07** avec filets fins, tableaux historiques à lignes hairline avec
badges numérotés (dernière étape en doré), **pastilles de statut** (Réglé / En cours / Pas encore réglé),
notice **⚠ URGENT** surlignée en rouge, filigrane « Confidentiel », blocs de signature
« Fait à … , le … » et pied de page confidentiel.

**Chiffres responsables / Responsible figures :** tous les montants, dates, références et totaux sont composés
dans une police monospace à chiffres tabulaires et zéro barré/pointé (Consolas, SF Mono, Menlo, DejaVu…) —
alignement vertical parfait en colonne et aucune confusion possible entre 0/O, 1/7, 3/8.

## 🚀 Utilisation / Usage

1. Ouvrir `index.html` dans un navigateur (double-clic suffit — Chrome, Edge ou Firefox recommandé).
2. Remplir le formulaire à gauche ; l'aperçu du document se met à jour en direct à droite.
3. Cliquer sur **« ⬇ Télécharger PDF / Download PDF »**, puis dans la boîte d'impression du
   navigateur choisir **« Enregistrer au format PDF / Save as PDF »** comme destination.

> Aucune installation, aucun serveur ni connexion Internet requis. Tout se fait en local,
> aucune importation de données.

## 📋 Contenu de la fiche / Sheet content

| Section | FR / EN |
|---|---|
| En-tête entreprise | Raison Sociale, adresse, email, logo — *Company name, address, email, logo* |
| Document | Titre, référence, date — *Title, reference, date* |
| Profil du Bénéficiaire | **Ajout de photo** (locale), nom et prénoms, adresse — *Beneficiary profile, photo upload* |
| Informations du Dossier | Nom, adresse, **montant sollicité**, **mensualité**, devise — *File information* |
| Statut | **Historique chronologique numéroté** — ajoutez une case **à chaque fois que la procédure suit son cours** ; les étapes sont reclassées automatiquement par date (de la plus ancienne à la plus récente), la dernière en date est surlignée — *Status: numbered chronological history, latest step highlighted* |
| Forfait Assurance | Montant (par défaut **1 115 EUR**) et statut de règlement — *Insurance fee, default "not yet paid"* |
| Statuts Paiements effectués ou en cours | **Historique chronologique des frais à payer** : montant, devise, statut (réglé / en cours / pas encore réglé), **notice Urgente ⚠** et totaux réglé / non réglé — *Payment statuses: chronological fee list, urgent notice, totals* |
| Transmission à la Banque | **Historique chronologique** (N°, date, banque, information transmise) — *Transmission to the bank: chronological history* |
| Statut de la Transaction | **Historique chronologique** (N°, date, statut, détails) — *Transaction status: chronological history* |
| Pied de page | Zone de signature de l'Entreprise uniquement (cachet) — *Company signature area only* |

## 💾 Stockage local / Local storage

- Le brouillon est **enregistré automatiquement** dans le navigateur (localStorage).
- Le bouton **« 💾 Enregistrer »** archive le dossier courant ; il peut être rouvert plus tard
  via la section **« Archives Locales / Local Archives »**.
- Les photos sont lues, **redimensionnées et stockées localement** (aucun envoi réseau).
- **« ⟲ Réinitialiser »** vide le formulaire ; **« 🧪 Exemple »** charge des données de démonstration.

## 🖨 Astuce PDF / PDF tip

Dans la boîte d'impression : destination **« Enregistrer au format PDF »**, format **A4**,
marges par défaut, et cocher **« Graphiques d'arrière-plan »** pour conserver les teintes (filets, pastilles, surlignages).
