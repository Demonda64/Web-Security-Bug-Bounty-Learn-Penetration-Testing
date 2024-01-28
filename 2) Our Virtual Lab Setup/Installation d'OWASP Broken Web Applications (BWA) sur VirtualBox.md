# Installation d'OWASP Broken Web Applications (BWA) sur VirtualBox

OWASP BWA est une collection d'applications web intentionnellement vulnérables conçue pour apprendre les tests de sécurité des applications web.

## Prérequis

- Assurez-vous que VirtualBox est installé.
- Téléchargez le fichier OVA de OWASP BWA depuis le site officiel d'OWASP.

## Étapes d'installation

1. **Importer le fichier OVA dans VirtualBox** :
   - Ouvrez VirtualBox.
   - Allez dans le menu `Fichier` > `Importer un service virtuel...`.
   - Sélectionnez le fichier OVA de OWASP BWA téléchargé et suivez les instructions pour l'importer.

2. **Configurer la machine virtuelle importée** :
   - Après l'importation, sélectionnez la VM OWASP BWA dans VirtualBox.
   - Cliquez sur `Paramètres` pour ajuster les configurations si nécessaire (par exemple, la quantité de RAM).

3. **Démarrer OWASP BWA** :
   - Sélectionnez la VM OWASP BWA.
   - Cliquez sur `Démarrer` pour initialiser la machine virtuelle.

4. **Utiliser OWASP BWA** :
   - Une fois que la VM est démarrée, utilisez votre navigateur pour accéder aux applications web vulnérables fournies par OWASP BWA.
   - Vous pouvez souvent accéder à OWASP BWA via http://localhost ou http://[IP_VM] où `[IP_VM]` est l'adresse IP attribuée à la VM OWASP BWA.

## Notes complémentaires

- Vous devrez peut-être configurer les paramètres réseau de la VM pour assurer une bonne connectivité.
- Assurez-vous de ne pas exposer OWASP BWA sur un réseau non sécurisé car les applications sont vulnérables par conception.

