# WebCRM — Fiche de situation bénéficiaire / Beneficiary status sheet

Application web **100 % locale** (un seul fichier `index.html`, aucune dépendance, aucune donnée
envoyée sur Internet) permettant de produire une **situation sur un client / bénéficiaire d'un
programme financier**, avec **rendu bilingue Français / Anglais** et **export PDF téléchargeable**.

---

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
| Statut | Cases dynamiques à ajouter **à chaque fois que la procédure suit son cours** — *Status* |
| Forfait Assurance | Montant (par défaut **1 115 EUR**) et statut de règlement — *Insurance fee, default "not yet paid"* |
| Transmission à la Banque | Cases dynamiques (date, banque, information transmise) — *Transmission to the bank* |
| Statut de la Transaction | Cases dynamiques (date, statut, détails) — *Transaction status* |
| Pied de page | Zones de signature entreprise / bénéficiaire — *Signature areas* |

## 💾 Stockage local / Local storage

- Le brouillon est **enregistré automatiquement** dans le navigateur (localStorage).
- Le bouton **« 💾 Enregistrer »** archive le dossier courant ; il peut être rouvert plus tard
  via la section **« Dossiers Enregistrés / Saved Files »**.
- Les photos sont lues, **redimensionnées et stockées localement** (aucun envoi réseau).
- **« ⟲ Réinitialiser »** vide le formulaire ; **« 🧪 Exemple »** charge des données de démonstration.

## 🖨 Astuce PDF / PDF tip

Dans la boîte d'impression : destination **« Enregistrer au format PDF »**, format **A4**,
marges par défaut, et cocher **« Graphiques d'arrière-plan »** si les bandeaux bleus n'apparaissent pas.
