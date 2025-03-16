# BDCC-IOC: Démonstration Spring IoC et Injection de Dépendances

## À propos
Ce projet démontre les principes d'Inversion de Contrôle (IoC) et d'Injection de Dépendances (DI) en utilisant Spring Framework.

## Structure du Projet

### Couche DAO
- Interface IDao avec méthode getData()
- DaoImpl: version base de données (34)
- DaoImplV2: version capteurs (12)

### Couche Métier
- Interface IMetier avec méthode calcul()
- MetierImpl: utilise IDao pour les calculs

### Couche Présentation
- Pres1: instanciation statique
- Pres2: instanciation dynamique (config.txt)
- PresSpringXML: configuration XML
- PresSpringAnnotation: configuration par annotations

## Principes Illustrés
- Couplage faible via interfaces
- Injection par constructeur et setter
- IoC avec Spring Framework

## Configuration Spring
- Annotations: @Repository, @Service, @Qualifier
- XML: beans dans config.xml

## Exécution
1. Statique: lancer Pres1
2. Dynamique: créer config.txt puis lancer Pres2
3. Spring XML: lancer PresSpringXML
4. Spring Annotations: lancer PresSpringAnnotation

## Prérequis
- Java 23
- Maven
- Spring 6.2.3

## Résultat
Avec DaoImplV2: environ -38.24
