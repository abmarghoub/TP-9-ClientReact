# TP 9 : Client React pour API REST

## 1. Objectif du TP

L’objectif de ce TP est de développer une application complète Full Stack composée de :

* Un backend Spring Boot exposant une API REST pour gérer des comptes bancaires (affichage, création).
* Un frontend React permettant d’afficher les comptes et d’ajouter de nouveaux comptes via un formulaire.
* Une communication entre React et Spring Boot grâce à un endpoint configuré dans un fichier centralisé.

Ce TP permet de maîtriser :

* La création d’API REST avec Spring Boot.
* L'utilisation d’une base de données H2 en mémoire.
* L’appel d’API REST depuis React via Axios.
* La structuration d’une application React en composants réutilisables.

---

## 2. Architecture du TP

### 2.1 Stack Technologique

| Layer           | Technologie         | Description                            |
| --------------- | ------------------- | -------------------------------------- |
| Backend         | **Spring Boot**     | Framework Java pour créer une API REST |
| Base de données | **H2 Database**     | Base en mémoire pour tests             |
| Frontend        | **React JS**        | Interface utilisateur web              |
| Client HTTP     | **Axios**           | Appels HTTP vers le backend            |
| Styling         | **Bootstrap 5**     | Mise en forme de l’UI                  |
| Outils          | Maven, Node.js, npm | Build & gestion des dépendances        |


### 2.2 Structure du projet

#### **Backend (Spring Boot)**

<img width="485" height="679" alt="image" src="https://github.com/user-attachments/assets/333f382c-42f7-4fd6-a730-58b12d9cf388" />

#### **Frontend (React)**

<img width="389" height="638" alt="image" src="https://github.com/user-attachments/assets/99c1f3bb-e64f-472d-bf09-58243bc744c7" />


---

## 3. Résultat Attendu

### **Formulaire d’ajout de compte**

<img width="852" height="818" alt="tp9-al" src="https://github.com/user-attachments/assets/83d4b374-5cdf-4f21-a8ae-5b248895a93e" />

<img width="868" height="492" alt="tp9-ala" src="https://github.com/user-attachments/assets/66564ed8-6b55-4380-90eb-569c5b123ae2" />
<img width="868" height="867" alt="tp9-aj" src="https://github.com/user-attachments/assets/ae832304-3087-44d1-866f-34528048cfdb" />


###  Processus global

1. L'utilisateur remplit le formulaire → clique sur **Ajouter**.
2. Une requête API POST est envoyée :

   ```
   POST http://localhost:8082/banque/comptes
   ```
3. Le compte apparaît dans la liste en dessous.
<img width="848" height="673" alt="tp9-h2" src="https://github.com/user-attachments/assets/b2a894d7-1a09-4dac-bae9-5281ba7ea5e2" />


---
## Auteur
**Réalisé par :** Abla MARGHOUB <br>
**Encadré par :** Pr. Mohamed LACHGAR<br> 
**Module :** Techniques de Programmation Avancée<br> 
**Cours :** Architecture Microservices : Conception, Déploiement et Orchestration<br>
**Établissement :** École Normale Supérieure - Université Cadi Ayyad<br>
