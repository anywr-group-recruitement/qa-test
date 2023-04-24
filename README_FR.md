[Version anglaise](README.md)

# Bienvenue à l'examen Anywr Software Tester !
Avant de commencer, veuillez lire attentivement les instructions suivantes :

- Cet examen est conçu pour évaluer vos connaissances et vos compétences dans divers aspects des tests de logiciels, tels que les tests manuels, l'automatisation des tests, les tests de bases de données, les tests d'API et la planification des tests.
- Veuillez lire attentivement chaque question et fournir des réponses claires, concises et bien organisées.
- Bien que nous vous encouragions à traiter tous les sujets de l'examen, nous comprenons que vous n'ayez pas d'expertise dans tous les domaines. Si vous n'êtes pas en mesure d'accomplir une tâche ou de répondre à une question, ne vous inquiétez pas.
  répondre à une question, ne vous inquiétez pas. Il est plus important de mettre en valeur vos points forts et de fournir des réponses réfléchies dans les domaines où vous êtes le plus à l'aise.

### Test manuel

En tant que testeur AQ, vous êtes chargé de tester manuellement les pages de la mission freelance. L'application
permet aux utilisateurs de rechercher une mission et de poser leur candidature.

URL : <https://www.anywr.frl/en/freelance/freelance-mission>

**Tâche:**

- Listez les cas de test que vous pouvez rédiger pour la section de la mission de recherche
- Mentionnez les scénarios positifs et négatifs. Organisez la liste des cas de test par priorité.
- Suggérez des améliorations qui pourraient améliorer l'expérience de l'utilisateur ou la fonctionnalité. (si elles existent)
- Identifiez et signalez tout bogue découvert, le cas échéant.

### API Testing - "Create Booking" Endpoint Validation" (Test de l'API - Validation du point de terminaison "Create Booking")

En tant que testeur QA, vous êtes chargé de tester l'API Restful Booker, une API RESTful simple qui permet aux utilisateurs de gérer les réservations d'hôtel.
qui permet aux utilisateurs de gérer les réservations d'hôtel. Vous vous concentrez principalement sur le point de terminaison "Create Booking",
qui permet aux utilisateurs de créer de nouvelles réservations.

Utilisez le lien suivant pour la méthode API Booking :

<https://restful-booker.herokuapp.com/apidoc/index.html#api-Booking-CreateBooking>

- Configurez l'API Restful Booker dans un outil de test d'API populaire (par exemple, Postman, Insomnia ou tout autre outil de votre choix).
- Testez le point de terminaison "Create Booking" avec différents cas de test, couvrant des scénarios positifs, négatifs et limites.
- Identifiez et listez les bogues ou les problèmes détectés au cours du processus de test. Fournissez une brève description de chaque bogue, y compris le cas de test, les étapes de reproduction, le résultat attendu et le résultat réel.

### Test de bases de données - Enregistrement de l'utilisateur et validation de la connexion

#### Examen 1

Vous travaillez sur une application web qui utilise une base de données relationnelle pour stocker les informations relatives aux utilisateurs.
L'application permet aux utilisateurs de s'inscrire et de se connecter.

La table suivante contient les données des utilisateurs :

```
Table des utilisateurs
- Id (INT, clé primaire, auto-incrément)
- Email (VARCHAR, unique)
- Mot de passe (VARCHAR)
```

***Écrivez des requêtes SQL pour tester les scénarios suivants:***

- Ajoutez un nouvel utilisateur à la table User.
- Vérifier que le nouvel utilisateur est ajouté à la table Users avec l'adresse électronique et le mot de passe corrects après l'enregistrement.
- Vérifier qu'un utilisateur ne peut pas être ajouté avec une adresse électronique qui existe déjà dans la table Utilisateurs.

#### Examen 2

Vous avez trois tables (Clients, Commandes et Employés) comme ci-dessous :

**Customers:**

| customer_id | customer_name  | customer_email          |
|-------------|----------------|-------------------------|
| 1           | John Doe       | john.doe@mail.com       |
| 2           | Jane Smith     | jane.smith@mail.com     |
| 3           | Bob Johnson    | bob.johnson@mail.com    |
| 4           | Sarah Williams | sarah.williams@mail.com |
| 5           | Diana smith    | Diana.smith@mail.com    |
| 6           | Will storm     | Will.storm@mail.com     |

**Orders:**

| order_id | customer_id | order_date | order_amount |
|----------|-------------|------------|--------------|
| 1        | 1           | 2022-04-16 | 100.00       |
| 2        | 1           | 2022-04-15 | 50.00        |
| 3        | 2           | 2022-04-14 | 75.00        |
| 4        | 3           | 2022-04-13 | 200.00       |
| 5        | 4           | 2022-04-12 | 150.00       |
| 6        | 6           | 2022-04-12 | 175.00       |
| 7        | 1           | 2022-01-12 | 120.60       |


**Employee:**

| employee_id | employee_name  | department_name | salary |
|-------------|----------------|-----------------|--------|
| 1           | John Smith     | Sales           | 50000  |
| 2           | Jane Doe       | Marketing       | 55000  |
| 3           | Bob Johnson    | Sales           | 60000  |
| 4           | Sarah Williams | Marketing       | 65000  |
| 5           | James Lee      | Finance         | 70000  |

***Questions:***

- Écrire une requête pour trouver les 4 premiers clients qui ont effectué le montant total d'achat le plus élevé au cours du dernier mois.
- Écrire une requête pour joindre deux tables, "Clients" et "Commandes", et renvoyer les noms de tous les clients qui ont passé une commande au cours de l'année écoulée.
- Écrire une requête pour calculer le salaire moyen des employés dans chaque département et renvoyer les résultats triés par ordre décroissant du salaire moyen.


### Questions de codage :

**Questions à options multiples:**

1 - En considérant le code ci-dessous, choisissez la sortie correcte :
  - var a = “5”;
  - var b = “5”;
  - var sum = a+b;
  - console.log(sum);

**sortie :**
- “a+b”
- 10
- “55”


2 - Quelle méthode utiliseriez-vous pour convertir une chaîne de caractères en majuscules ?
  - toLowerCase()
  - toUpperCase()
  - capitalize()
  - upper()


3 - En considérant le code ci-dessous, choisissez la sortie correcte :

- var x = [1, 2, 3];
- console.log(x.length);

**sortie :**
- 0
- 1
- 2
- 3

### Tests d'automatisation :

#### Section 1 : Questions à choix multiples :

1- Vous devez tester un champ n'acceptant que des nombres entre 2 et 1000, chaque cas de test ne peut vérifier qu'un seul nombre.
- Test 1 avec le nombre (-1).
- Test 2 avec le nombre (1).
- Test 3 avec le nombre (500).

Laquelle des réponses ci-dessous est correcte:
- Le cas de test 1 est un cas de test négatif, les cas de test 2 et 3 sont positifs.
- Tous les cas de test sont positifs.
- Les cas de test 1 et 2 sont des cas de test négatifs, le test 3 est un test positif.
- Tous les cas de test sont négatifs.

2- Qu'est-ce qu'une assertion dans les tests d'automatisation de l'interface utilisateur ?

- Pour confirmer un résultat de test précédent
- Rapport de résultats de tests
- Résumé des étapes du test
- Résumé des résultats des cas de test

3- Qu'est-ce qu'un test de régression dans les tests d'automatisation de l'interface utilisateur ?

- Tester une nouvelle fonctionnalité isolée du reste de l'application.
- Tester le même ensemble de cas de test à plusieurs reprises pour s'assurer qu'aucun nouveau bogue n'a été introduit.
- Tester l'application dans différentes conditions de réseau.
- Tester l'application sous différents navigateurs.

## Section 2 :

En tant que testeur AQ, vous êtes chargé d'automatiser un test d'interface utilisateur pour la fonctionnalité "Mot de passe oublié" sur la page de connexion du groupe Talent Anywr.
sur la page de connexion du groupe Talent Anywr. L'application permet aux utilisateurs de réinitialiser leur mot de passe en
en fournissant leur adresse e-mail.

URL : <https://talent.anywr-group.com/en/login>

- Choisissez votre outil d'automatisation préféré (par exemple, Selenium WebDriver, Cypress, TestCafe) et créez un script de test pour automatiser le cas de test suivant :
- Vérifier que la fonctionnalité "Mot de passe oublié" envoie un courriel de réinitialisation du mot de passe à l'adresse électronique enregistrée de l'utilisateur. (Note : ignorez le test de l'e-mail)
- Signalez tout bogue trouvé au cours du processus de test. (Le cas échéant)
- Suggérer des améliorations à la fonctionnalité "Oubli de mot de passe" qui pourraient améliorer l'expérience de l'utilisateur ou la fonctionnalité. (Le cas échéant)

***Si vous avez de l'expérience dans les domaines des tests de performance, de charge, de stress ou de sécurité, pourriez-vous nous donner des détails sur votre expérience ?
Si vous avez de l'expérience dans les domaines des tests de performance, de charge, de stress ou de sécurité, pourriez-vous fournir des détails sur vos projets pertinents, vos réalisations et votre expertise dans ces domaines ?
et votre expertise dans ces domaines ?***

**Bonne chance !
