BOT DISCORD TIERS + QUEUE

1. Installe Python 3.10 ou plus récent.
2. Installe les dépendances : pip install -r requirements.txt
3. Renomme .env.example en .env.
4. Dans .env, remplis DISCORD_BOT_TOKEN et TESTER_ROLE_ID.
5. Lance : python bot.py

TESTER_ROLE_ID est l'ID du rôle Discord autorisé à utiliser /tiers-set.
TICKET_CATEGORY_ID est l'ID de la catégorie où les tickets privés de la queue seront créés. Le système de queue, les boutons rejoindre/quitter, les tickets privés et leur bouton de fermeture sont conservés.
Pour copier l'ID du rôle sur Discord : active le mode développeur, ouvre les paramètres du rôle, puis Copie l'identifiant.
Le bot doit avoir les permissions Voir le salon, Envoyer des messages et Intégrer des liens.
Dans le portail développeur Discord, active l'installation sur serveur et l'application commands si nécessaire.

La commande /tiers-set demande le pseudo Minecraft, puis le mode, puis le tier obtenu.
Le résultat est publié dans le salon où la commande a été lancée. Le tier précédent est récupéré dans queue.db lorsqu'il existe pour ce pseudo et ce mode ; sinon il affiche Unranked.
Le champ région est réglé sur EU et le skin est chargé via mc-heads.net. Les tiers disponibles vont de HT1 à LT5 uniquement : HT1, LT1, HT2, LT2, HT3, LT3, HT4, LT4, HT5, LT5.

Ne partage jamais le fichier .env ou ton token. Si ton token a été partagé publiquement, régénère-le dans le portail développeur Discord.
