# AutoLoc - Plateforme de gestion de location de véhicules multi-agences

**Étude de cas** : Atelier 0 — Mise en place de l'environnement de développement  
**Département** : Architecture des Systèmes d'Information (UP ASI)  
**Établissement** : ESPRIT

## Objectifs du projet

AutoLoc est une application Spring Boot complète visant à modéliser et gérer le cycle de location de véhicules à travers plusieurs agences. Le système doit_SUPPORTER les opérations suivantes :

- Enregistrement et gestion des **clients** (particuliers et entreprises)
- Gestion des **agents d'agence** et des **responsables d'agence**
- Catalogue des **véhicules** (types, disponibilité, statut)
- Traitement des **locations** (mise en location, retour, prolongation)
- Facturation et suivi des paiements
- Tableau de bord administratif

## Acteurs identifiés

| Acteur | Rôle |
|--------|------|
| **Client** | Réserve, modifie ou annule un véhicule en location |
| **Agent d'agence** | Gère le catalogue véhicules, traite les locations |
| **Responsable d'agence** | Supervise l'agence, autorise les actions stratégiques |
| **Administrateur** | Paramétrage global, gestion des utilisateurs, états financiers |

## Stack technique récapitulative

| Catégorie | Outils / Bibliothèques |
|-----------|----------------------|
| Langage / Build | Java 17+, Maven 3.8+ |
| Framework | Spring Boot, Spring Data JPA, Spring MVC, Spring AOP, Spring Scheduler |
| Base de données | MySQL 8.x (développement), H2 en mémoire pour les tests |
| Productivité | Lombok, SLF4J/Logback, MapStruct (mapping DTO, optionnel) |
| Documentation API | springdoc-openapi (Swagger UI) |
| Tests | JUnit 5, Mockito, MockMvc, JaCoCo |
| Qualité | SonarLint (IDE), SonarQube (optionnel) |
| Outillage | Git/GitHub, Postman, IntelliJ IDEA Ultimate |

## Checklist Atelier 0 — Mise en place de l'environnement

Tâche / Livrable | Fait ✔
---------------- | -----
JDK 17 installé et vérifié (`java -version`) | ☐
IntelliJ IDEA Ultimate installé et licence étudiante activée | ☐
MySQL installé, service démarré, base `autoloc_db` créée | ☐
Postman installé | ☐
Compte / organisation Git créé, dépôt `AutoLoc` initialisé | ☐
README.md v0 rédigé : objectifs du projet + acteurs identifiés (Client, Agent, Manager, Administrateur) | ☐
Capture d'écran ou preuve de l'environnement fonctionnel jointe au dépôt | ☐

## Étapes suivantes (Ateliers 1+)

1. Modélisation JPA / entités (Client, Vehicule, Location, Agence)
2. Répositories Spring Data JPA
3. Contrôleurs REST (endpoints CRUD)
4. Tests unitaires et intégration (JUnit 5 + MockMvc)
5. Documentation API via Swagger UI (springdoc-openapi)
6. Configuration SonarQube et qualité continue

---

**Bonne installation, et à vous de jouer !**