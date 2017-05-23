NAME:
      Backup_RBD est un outil de sauvegarde ProxmoxVE / CephRBD

SYNOPSIS:

      Backup_RBD OPTION [PARAMETERS]=[OPTIONS]

OPTIONS:

      Backup_RBD version
          Affiche la version du programme

      Backup_RBD help
          Affiche cette page et sort du programme

      Backup_RBD create
          Créer une tâche de sauvegarde planifiée

      Backup_RBD remove
          Supprime une tâche de sauvegarde existante

      Backup_RBD enable
          Active une tâche de sauvegarde existante

      Backup_RBD disable
          Désactive une tâche de sauvegarde existante

      Backup_RBD backup
          Sauvegarde une ou plusieurs VMs

      Backup_RBD restore
          Restaure une ou plusieurs sauvegardes

      Backup_RBD list
          Liste les sauvegardes existante pour une VM

PARAMETERS:

      --vmid=<string>
          Spécifie le ou les numéros de VM à sauvegarder (si plusieurs séparer les vmids par une virgule)
          \"all\" pour un backup de toutes les VMs

      --dayfull=<string>
          Spécifie le jour de la semaine où le backup complet doit être réalisé

      --keep=<int>
          Spécifie le nombre de sauvegarde à conserver dans le backupdir

      --backupdir=<string>
          Spécifie le repertoire de destination des sauvegardes

      --mail=<string>
          Spécifie une ou plusieurs adresse mail pour l\'envoi des logs du jour
      --compress=<string>
          Active ou non la compression des sauvegardes (on/off, default=on)

SETUP:

      Copy the Backup_RBD into one of thoose directory (/usr/local/sbin:/usr/local/bin:/sbin:/bin:/usr/sbin:/usr/bin)

CONTACT:
      skadia@protonmail.com
