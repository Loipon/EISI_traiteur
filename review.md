Review de code Titouan Plomb : 
https://github.com/t2plbonnet/EISI_traiteur.git


- 1. Boucle sur les données CSV : le fichier CSV est parcouru plusieurs fois sans être réinitialisé, ce qui entraîne une erreur après la première itération.

- 2. Traitement des températures : les températures sont converties en float, mais ensuite en int, ce qui perd en précision .

- 3. Liste des températures : la liste température est accumulée sans être vidée après chaque traitement de chambre froide.

- 4. Affichage redondant : la liste température est appelé à chaque ajout dans la liste donc la sortie affiche mal

- 5. Gestion des erreurs : aucune gestion des erreurs n'est prévue pour les cas où le fichier CSV est introuvable ou les données sont mal formées.

