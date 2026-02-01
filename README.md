## Objectif

Mettre en place une surveillance ciblée du service **DNS Server** sur une machine **Windows Server** à l’aide d’une vue personnalisée dans l’**Event Viewer**.

---

## Environnement

- **Machine virtuelle** : Windows Server  
- **Rôle installé** : DNS Server  
- **Outil** : Event Viewer  

---

## Configuration de la vue personnalisée

### Journal surveillé
- `Microsoft-Windows-DNS-Server`

### Niveaux d’événements
- Critique  
- Erreur  
- Avertissement  
- Information (démarrages / arrêts)

### Sources d’événements
- `DNS-Server-Service` (journal DNS-Server)

### IDs d’événements ciblés
- **2** : Démarrage du service DNS  
- **4** : Arrêt du service DNS  
- **409** : Erreur de résolution de nom  
- **501–502** : Échec de chargement de zone  
- **6001–6002** : Problèmes de réplication DNS  
