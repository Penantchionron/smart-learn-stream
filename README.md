Smart Learn Stream – Mini plateforme de streaming vidéos

##  Description du projet

Smart Learn Stream est une mini-plateforme de streaming éducatif développée pour simuler un parcours utilisateur complet (Client Experience – CX) dans le cadre d'un projet fictif. Elle permet de diffuser des vidéos éducatives gratuites via une interface moderne, responsive et interactive.

Le projet intègre un front-end dynamique avec Vue.js (Inertia), un back-end robuste via Laravel, une base stylisée grâce à Tailwind CSS et un template UI personnalisé TailDashboard. Le parcours inclut la découverte des vidéos, une fiche descriptive, ainsi qu’un système de filtrage par catégories.

##  Objectifs fonctionnels

* ✅ Interface web responsive et ergonomique
* ✅ Affichage des vidéos via YouTube Embed ou vidéos locales
* ✅ Page d’accueil listant les vidéos (titre, image, catégorie)
* ✅ Fiche vidéo avec description et lecteur intégré (modal ou page)
* ✅ Filtrage par thème ou catégorie
* ✅ (Facultatif) Système d’abonnement utilisateur
* ✅ (Facultatif) Paiement mobile

##  Stack technique utilisée

| Élément         | Technologie               | Justification                                                         |
| --------------- | ------------------------- | --------------------------------------------------------------------- |
| Frontend        | Vue.js (Vite, Inertia.js) | SPA performant, rendu rapide, couplé à Laravel via Inertia            |
| Backend         | Laravel (PHP 8.2.12 +)    | Framework robuste, sécurité intégrée,API RESTFull,Gestion d'authentification support Inertia.js,vite |
| UI/Design       | Tailwind CSS + TailTubeUI | Design moderne, responsive et personnalisable                               |
| Base de données | MySQL                     | Simple à mettre en œuvre , simple pour faire des tests
| Hébergement     | Render.com                | Déploiement rapide, CI/CD intégré                                       | 

##  Fonctionnalités développées

* ✅ Interface d’accueil listant toutes les vidéos
* ✅ Chargement dynamique des vidéos (YouTube embed)
* ✅ Système de filtrage par catégorie/thème
* ✅ Fiche vidéo avec lecteur + description en modal
* ✅ Interface responsive (mobile/tablette/desktop)
* ✅ Système d’inscription et de connexion (Dashboard utilisateur connecté)
* ✅ Dashboard Admin (Ajout/Modification/Suppression de vidéos)
* ✅ Système d'abonnement (prévu en extension)
* ✅ Paiement mobile (prévu en extension)

##  Instructions d'installation

### Prérequis

* Node.js (v20.x ou +)
* Git (v2.x ou +)
* Composer (v2.8.8 ou +)
* PHP (>= 8.2.12)
* MySQL (ou MariaDB)

### Étapes d'installation locale

1. Cloner le projet

```bash
git clone https://github.com/Penantchionron/smart-learn-stream.git
```

2. Installation

```bash
cd smart-learn-stream
composer install
npm install 
cp .env.example .env
php artisan key:generate
code .
```
![Installation](https://github.com/user-attachments/assets/5d32f66a-9823-4c88-907a-dbc05163380e)


3. Créer la base de données et configurer `.env`

```
DB_DATABASE=smartlearn
DB_USERNAME=your_user // root si c'est MySQL
DB_PASSWORD=your_password // pas de mot de pas si c'est MySQL
```
![Configuration](https://github.com/user-attachments/assets/dba7ddc9-1b62-4a5a-8468-cf13cb65fa9f)


4. Démmarer le serveur et Exécuter les migrations et les seeders

```bash
php artisan migrate --seed
```
![demarrer le serveur](https://github.com/user-attachments/assets/dddcde7c-2f59-41e5-935c-bf3585f9f969)


### Lancer Vite (compiler le frontend) et ### Lancer le serveur de développement de l'application 

```bash
npm run dev
npm run build 
php artisan serve
```
![Capture d'écran 2025-05-12 091730](https://github.com/user-attachments/assets/a13c4fa9-9353-4e9c-aae9-3dee32090f32)


5. tapper dans le navigateur : http://127.0.0.1:8000

#### 🧑‍💼 Site Démo
![Page d'accueil](https://github.com/user-attachments/assets/f1a32184-1db3-455d-8a31-4d35f651146b)
![Dashoard](https://github.com/user-attachments/assets/d7e802c0-ed48-41a4-88b8-982e975dbd3a)
![mobile](https://github.com/user-attachments/assets/a9aaba4b-ebdb-451b-9824-4e1363c3adcc)
![lecture](https://github.com/user-attachments/assets/4cb98831-5da0-418c-9b1a-39c4db2ded12)
![ThèmeN](https://github.com/user-attachments/assets/cbe0674b-3ec7-4a6b-af6e-9bb531d7df7f)

Lien pour tester ici 👉 bientot

##  Documentation technique 

👉 [https://github.com/Penantchionron/smart-learn-stream/main/docs/plan-technique.md ](https://github.com/Penantchionron/smart-learn-stream/blob/main/docs/plan-technique.md)
