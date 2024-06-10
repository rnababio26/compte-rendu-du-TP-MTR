# compte-rendu-du-TP-MTR
TITRE：Conception et Développement d'un Système Temps Réel et Multi-tâche : Gestion Automatisée de Téléviseurs dans une Maison Intelligente (Via un ESP32 et l'OS FreeRTOS) (Programmation Concurentielle).


memebre du groupes :ABABIO RAWLINGS NDANGOh
liens :https://wokwi.com/projects/398796544238587905)
resumé du projet:
Le système de gestion automatisée de téléviseurs dans une maison intelligente utilisant un ESP32 et FreeRTOS est un système temps réel et multi-tâche. FreeRTOS permet la gestion des tâches avec des priorités et des délais prédictibles, tandis que l'ESP32 offre les capacités nécessaires pour exécuter des opérations concurrentes. La modélisation par Réseau de Petri illustre le flux du système : depuis l'état initial d'attente d'un événement, passant par la détection, le traitement et l'exécution de l'action, jusqu'à l'état final de préparation pour un nouvel événement. Cette modélisation démontre comment le système répond de manière efficace et fiable aux événements en temps réel.

Question 1 : Est-ce que ce système est un système temps réel et multi-tâche ? Justifiez. 
réponse. Oui, ce système est un système temps réel et multi-tâche.
          car Ce système, utilisant un ESP32 avec FreeRTOS pour la gestion automatisée de téléviseurs dans une maison intelligente, est clairement un système temps réel et multi-tâche. Il répond aux exigences d'un système temps réel en garantissant que les tâches critiques soient effectuées dans des délais déterminés et utilise les capacités multi-tâches de FreeRTOS et de l'ESP32 pour gérer simultanément plusieurs tâches, assurant ainsi un fonctionnement fluide et efficace.
  Question2:Réalisez la modélisation par Réseau de Petri de ce système
  (voir pdf)
 Question 3.Grâce au Réseau de Petri, énumérez vos tâches ainsi que leurs propriétés
 P0 (Système en attente) : Le système commence dans cet état, en attente de la détection d'un événement.
T1 (Détection d'événement) : Lorsqu'un capteur détecte un événement, il déclenche cette transition.
P1 (Événement détecté) : Indique que l'événement a été détecté et attend le traitement.
T2 (Début du traitement) : La transition vers le traitement de l'événement commence.
P2 (Traitement en cours) : Le système traite l'événement détecté (par exemple, déterminer quel téléviseur allumer).
T3 (Exécution de l'action) : Déclenche l'exécution de l'action nécessaire (par exemple, envoyer un signal pour allumer le téléviseur).
P3 (Action en cours) : Représente que l'action est en cours d'exécution.
T4 (Fin de l'action) : Transition lorsque l'action est terminée.
P4 (Système prêt) : Le système retourne à l'état de préparation pour détecter un nouvel événement.
question 4.:https://wokwi.com/projects/398796544238587905)
