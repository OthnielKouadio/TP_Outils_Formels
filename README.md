Rapport Final du Projet : Système de Contrôle d'Accès

Le projet vise à modéliser, simuler et valider un système de contrôle d'accès basé sur des concepts de logique formelle, d'automates finis, et de circuits logiques. Il met en œuvre les règles fondamentales d'un tel système : vérification d'une carte et d'un code, gestion des états (accès accordé, refusé, ou alarme), et simulation des comportements via des outils programmatiques en Java.

1. Spécification et Modélisation du Système
1.1 Spécification des règles
Les règles fondamentales du système ont été formalisées comme suit :

Règle 1 : L'accès est accordé si et seulement si la carte est valide et le code est correct.
Règle 2 : L'accès est refusé si l'une des deux conditions (carte valide ou code correct) est fausse.
Règle 3 : Une alarme est déclenchée si la carte est invalide ou si le code est incorrect.
Ces règles ont été implémentées dans la classe Verification pour assurer la conformité avec les spécifications.

1.2 Modélisation avec un automate
Un automate a été conçu pour représenter les différents états du système :

q0 : Attente d'une carte.
q1 : Vérification du code.
q3 : Accès accordé.
q4 : Accès refusé ou alarme déclenchée.
Chaque état et transition a été défini clairement, et le système a été simulé pour gérer dynamiquement les entrées utilisateur (présentation d'une carte et saisie d'un code).

2. Implémentation en Java
2.1 Vérification des Règles
Le fichier Verification.java regroupe les règles de sécurité sous forme de conditions booléennes pour garantir leur respect. Les messages associés confirment que les états et transitions respectent les spécifications.

2.2 Automate de Contrôle d'Accès
Le fichier Automate.java modélise un automate fini déterministe pour simuler les états et les transitions :

Les entrées utilisateur déterminent les changements d'état.
Les messages affichés dans chaque état permettent une interaction en temps réel et une validation des règles du système.
3. Validation du Système
Le système a été validé à travers des scénarios spécifiques :

Une carte valide suivie d’un code correct permet l’accès.
Une carte invalide ou un code incorrect refuse l’accès et/ou déclenche une alarme.
Les règles ont été vérifiées en utilisant des conditions booléennes, garantissant que les états sont correctement modélisés et que les transitions sont cohérentes.

4. Défis et Solutions
Défis rencontrés :
Modélisation logique des règles pour éviter la redondance.
Gestion des différents scénarios utilisateurs avec des transitions d’états bien définies.
Validation systématique de chaque règle pour garantir l'alignement avec les spécifications.
Solutions apportées :
Utilisation de structures conditionnelles (if, switch) pour une gestion claire des transitions d’états.
Simplification des règles logiques pour éviter la duplication et améliorer la lisibilité du code.
Simulation en temps réel avec des entrées utilisateur pour valider les comportements attendus.
5. Conclusion et Recommandations
Le projet a permis de :

1°Spécifier, modéliser et implémenter un système de contrôle d’accès fonctionnel.
2°Valider la conformité des états et des transitions via des simulations en Java.
3°Développer des compétences en logique propositionnelle, automates finis, et vérification formelle.
Recommandations pour une amélioration future :
4°Ajouter des fonctionnalités supplémentaires : Par exemple, la gestion des tentatives multiples ou la journalisation des accès.
Inclure une interface utilisateur graphique pour améliorer l’expérience utilisateur.
4°Tester le système avec des outils de vérification formelle pour garantir une robustesse accrue face à des scénarios complexes.
