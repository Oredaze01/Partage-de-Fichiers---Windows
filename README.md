# Partage-de-Fichiers---Windows

### Procédure pour la configuration et les testing de partage de fichiers


1. Installe le rôle Serveur de fichiers


![[PartageDeFichier-Windows-1.png]](Ressources/PartageDeFichier-Windows-1.png)



2. Crée un dossier "Documents_Entreprise" à la racine du disque C:


![[PartageDeFichier-Windows-2.png]](Ressources/PartageDeFichier-Windows-2.png)


3. Configure un partage nommé "Docs" pour ce dossier

Clique droit sur le dossier « Documents_Entreprise », aller dans propriété, puis propriété avancée et changer le share name en « Docs ».


![[PartageDeFichier-Windows-3.png]](Ressources/PartageDeFichier-Windows-3.png)



4. Crée trois sous-dossiers : "RH", "Comptabilité" et "Direction"


- Création de trois sous-dossiers

Allez dans les option share du dossier « Documents_Entreprise » et creer les trois sous dossiers comme demandé :


![[PartageDeFichier-Windows-4.png]](Ressources/PartageDeFichier-Windows-4.png)



![[PartageDeFichier-Windows-4.1.png]](Ressources/PartageDeFichier-Windows-4.1.png)








5. Configure les permissions NTFS et de partage pour que :
    - Le groupe "RH" ait un accès en lecture/écriture au dossier "RH"


![[PartageDeFichier-Windows-5.1.png]](Ressources/PartageDeFichier-Windows-5.1.png)



    - Le groupe "Comptabilité" ait un accès en lecture/écriture au dossier "Comptabilité"



![[PartageDeFichier-Windows-5.2.png]](Ressources/PartageDeFichier-Windows-5.2.png)



    - Le groupe "Direction" ait un accès en lecture/écriture à tous les dossiers


![[PartageDeFichier-Windows-5.3.png]](Ressources/PartageDeFichier-Windows-5.3.png)



    - Tous les utilisateurs du domaine aient un accès en lecture seule au dossier "Documents_Entreprise"


![[PartageDeFichier-Windows-5.4.png]](Ressources/PartageDeFichier-Windows-5.4.png)


6. Utilise PowerShell pour lister tous les partages sur le serveur



![[PartageDeFichier-Windows-6.png]](Ressources/PartageDeFichier-Windows-6.png)




7. Sur un poste client Windows 10, configure un lecteur réseau pointant vers ce partage via PowerShell


![[PartageDeFichier-Windows-7vrai.png]](Ressources/PartageDeFichier-Windows-7vrai.png)



8. Teste l'accès depuis le poste client avec différents comptes utilisateurs
9. 
Test avec [wilder.rh@wilder.lan](mailto:wilder.rh@wilder.lan "mailto:wilder.rh@wilder.lan")


Je n'ai pas réussit a faire cette question...
