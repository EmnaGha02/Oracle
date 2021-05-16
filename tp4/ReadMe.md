# TP4


 ## DEMO 

 - **Créer les nouveaux utilisateurs comme suit:**  
      A) Equipe Dev :

      * [ username: dev1, password: dev1 ]
      * [ username: dev2, password: dev2 ]
      
      B) Equipe Test :

      * [ username: tester1, password: tester1 ]
      * [ username: tester2, password: tester2 ]
     
     
     C) Equipe DevSecOps :      
      * [ username: devsecops1, password: devsecops1 ]
      * [ username: devsecops2, password: devsecops2 ]


```sql
---
```
  --->  **Une fois qu'un utilisateur est créé, le DBA peut octroyer des privilèges de système spécifiques à cet utilisateur.**
 

  - **Attribuer les privilèges ci-dessous à l'utilisateur dev1 :** 
 
     * Création de procédures stockées.
     * Création de vue.
     * Création de séquence.
     * Création de session.
     * Création,lecture, modification de structure et suppression de tables.

```sql
---
```

¤   **Une fois qu'un utilisateur est créé, le DBA peut octroyer des privilèges de système spécifiques à cet utilisateur.**
 
 
   - **Révoquer tous les privilèges associès à l'utilisateur dev1 :** 

```sql
---
```

 
  - **Créer des rôles dédiés pour chaque Equipe d'utilisateurs en réspectant les critères suivants** 

      A) Le rôle de l'équipe Dev permet de:

      * Création de procédures stockées.
      * Création de vue.
      * Création de séquence.
      * Création de session.
      * Création,lecture, modification de structure et suppression de tables.
      
      B) Le rôle de l'équipe Test permet de:

      * Se connecter à la base de données.
      * Création de session.
      * Lecture données de toutes les tables.
     
     C) Le rôle de l'équipe DevSecOps permet d'avoir tous les privilèges avec mode administrateur de la base:  

```sql
---
```
```sql
---
```
```sql
---
```
```sql
---
```


 
   - **Attribuer à chaque utilisateur, le rôle qui lui correspond:** 
  

```sql
---
```
```sql
---
```
```sql
---
```

   - **Limiter l'accès pour les testeurs de sorte qu'ils n'accèdent qu'à la table des employés "EMP":** 
  

```sql
---
```

 ```sql
---
```
 
 
 
   - **Autoriser tous les utilisateurs sur le système pour interroger les données de la table EMP :** 
  

 ```sql
---
```

**Retirer les privilèges attribuées aux admins, ainsi que les utilisateurs qui ont reçu leurs privilèges sur la table EMP par un membre de l'équipe devsecops:**

 
 
```sql
---
```


**Créer un profile de ressources dédié à l'équipe des développeurs avec les limitations suivantes:**
  * ***Nombre maximal de sessions permises par utilisateur:*** **illimité**
  * ***Nombre maximal de CPU par session:*** **10000**  
  * ***Nombre maximal de CPU par appel à la base :*** **1000**
  * ***Durée maximal en secondes d'une session:*** ***45*** 
  * ***Nombre maximal de lectures logiques par session utilisateur:*** ***Valeur par defaut***
  * ***Nombre maximal de lectures logiques par appel à la base:*** ***1000***
  * ***Taille maximale de l'SGA privée:*** ***25K***
  * ***Durée de vie en jours du mot de passe:*** ***60***
  * ***Nombre maximal de réutilisations de mot de passe:*** ***10***



```sql 
---
```




**Créer un profile de ressources dédié à l'équipe de test avec les limitations suivantes:**
  * ***Nombre maximal de sessions permises par utilisateur:*** **5**
  * ***Nombre maximal de CPU par session:*** **illimité**  
  * ***Nombre maximal de CPU par appel à la base :*** **3000**
  * ***Durée maximal en secondes d'une session:*** ***45*** 
  * ***Nombre maximal de lectures logiques par session utilisateur:*** ***Valeur par defaut***
  * ***Nombre maximal de lectures logiques par appel à la base:*** ***1000***
  * ***Taille maximale de l'SGA privée:*** ***25K***
  * ***Durée de vie en jours du mot de passe:*** ***60***
  * ***Nombre maximal de réutilisations de mot de passe:*** ***10***
```sql 
---
```

**Créer un profile de ressources dédié à l'équipe devsecops avec les limitations suivantes:**
  * ***Nombre maximal de sessions permises par utilisateur:*** **illimité**
  * ***Nombre maximal de CPU par session:*** **illimité**  
  * ***Nombre maximal de CPU par appel à la base :*** **3000**
  * ***Durée maximal en secondes d'une session:*** ***3600*** 
  * ***Nombre maximal de lectures logiques par session utilisateur:*** ***Valeur par defaut***
  * ***Nombre maximal de lectures logiques par appel à la base:*** ***5000***
  * ***Taille maximale de l'SGA privée:*** ***80K***
  * ***Durée de vie en jours du mot de passe:*** ***60***
  * ***Nombre maximal de réutilisations de mot de passe:*** ***10***

```sql 
---
```

  - **Attribuer à l'utilisateur "dev1", le profile qui lui correspond:** 
```sql
---
```

