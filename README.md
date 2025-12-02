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

![img.png](img.png)

#### **Frontend (React)**

![img_1.png](img_1.png)

---

## 3. Résultat Attendu

### **Formulaire d’ajout de compte**

![tp9-ala.png](../../Pictures/tp15/tp9-ala.png)
![tp9-al.png](../../Pictures/tp15/tp9-al.png)
![tp9-aj.png](../../Pictures/tp15/tp9-aj.png)



###  Processus global

1. L'utilisateur remplit le formulaire → clique sur **Ajouter**.
2. Une requête API POST est envoyée :

   ```
   POST http://localhost:8082/banque/comptes
   ```
3. Le compte apparaît dans la liste en dessous.
![tp9-h2.png](../../Pictures/tp15/tp9-h2.png)

---
