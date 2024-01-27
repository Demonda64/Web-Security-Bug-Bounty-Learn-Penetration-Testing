# Installation de Kali Linux sur VirtualBox

1. **Lancer VirtualBox** :
   - Ouvrez VirtualBox et sélectionnez 'Nouvelle' pour créer une nouvelle machine virtuelle.

2. **Configurer la nouvelle machine virtuelle** :
   - Nommez la VM (par exemple, "Kali Linux").
   - Choisissez 'Linux' comme type et 'Debian (64-bit)' comme version.
   - Cliquez sur 'Suivant' pour continuer.

3. **Attribuer la mémoire vive** :
   - Attribuez au moins 2048 MB de RAM pour de meilleures performances.
   - Cliquez sur 'Suivant' pour procéder.

4. **Créer un disque dur virtuel** :
   - Sélectionnez 'Créer un disque dur virtuel maintenant'.
   - Choisissez le type de fichier de disque dur (recommandé : VDI (VirtualBox Disk Image)).
   - Choisissez 'Dynamiquement alloué' pour un espace disque qui augmente au besoin.
   - Spécifiez la taille du disque (recommandé : 20 GB ou plus).
   - Cliquez sur 'Créer' pour finaliser la configuration de la VM.

5. **Monter l'image ISO de Kali Linux** :
   - Sélectionnez la machine virtuelle Kali Linux et cliquez sur 'Paramètres'.
   - Allez dans l'onglet 'Stockage', cliquez sur l'icône du disque vide sous 'Contrôleur: IDE'.
   - À droite, cliquez sur l'icône du disque pour choisir un fichier de disque.
   - Sélectionnez l'image ISO de Kali Linux téléchargée précédemment et cliquez sur 'Ouvrir'.

6. **Lancer l'installation** :
   - Avec la VM sélectionnée, cliquez sur 'Démarrer'.
   - Une fois démarré, suivez les instructions à l'écran pour installer Kali Linux.
   - Choisissez vos paramètres régionaux, disposition du clavier, et créez un utilisateur et un mot de passe.

7. **Finaliser l'installation** :
   - Après l'installation, éjectez l'image ISO de la configuration du stockage pour éviter le redémarrage de l'installation.
   - Redémarrez la VM.
   - Connectez-vous avec votre utilisateur et votre mot de passe créés.

Votre Kali Linux est maintenant installé et prêt à être utilisé dans VirtualBox.
