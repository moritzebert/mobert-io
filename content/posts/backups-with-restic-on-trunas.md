+++
title = 'Backups mit restic auf Trunas'
date = 2025-02-28T23:37:40+01:00
tags = ["Backup"]
draft = true
+++

Ich hatte bis vor kurzem keine wirkliche Backup Strategie für mein NAS. Ich repliziere die Daten regelmäßig auf eine externe Festplatte. Diese Festplatte befindet sich auch in meiner Wohnung und ist die einzige Kopie meiner Daten. Mittlerweile kann ich sagen, dass ich mein Homelab sehr produktiv nutze und auch wichtige Daten 
vorzugsweise auf meinem NAS speichere.  
Ich brauche also eine Methode, um disese Daten verschlüsselt in die Cloud zu übertragen und sie im Falle eines Ausfalls wiederherstellen zu können.

## Warum restic?

1. **Sicherheit**: Standardmäßige Verschlüsselung der Backups
2. **Effizienz**: Deduplication spart Speicherplatz und Bandbreite
3. **Einfachheit**: Einfache Nutzung über eine benutzerfreundliche Kommandozeile
4. **Automatisierbarkeit**: Einfach in Skripte oder Cronjobs integrierbar
5. **Flexibilität**: Unterstützt verschiedene Protokolle zur Übertragung (SFTP, REST, Rsync)

