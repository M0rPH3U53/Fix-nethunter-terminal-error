# Origine du problème

nhterm: **2025.4** (2025110400)

Magisk: **30.6**

Le problème au démarrage de `nhterm` est qu’il ne trouve pas de binaire `SU`

```
[android-su][ERROR] 'su' binary not found in path 
```

# Fix & compile 

APK Editor Studio: https://qwertycube.com/apk-editor-studio/download/

Apres avoir ouvert l'apk avec **APK Editor Studio** remplacer `/bin/su` par /`bin/bash` dans le fichier kali & enregistrer via **CTRL-S**

![2b41a08788805d3e18ef2943521f3ea0.png](../_resources/2b41a08788805d3e18ef2943521f3ea0.png)

&nbsp;

Ensuite aller dans `android-su` et supprimer les " " de “\${SU2\[@\]}” & enregistrer via **CTRL-S**

![23fb925e9afd2384273e7d82c59c24e7.png](../_resources/23fb925e9afd2384273e7d82c59c24e7.png)

&nbsp;

Fermer les 2 fenêtres des fichier et cliquer sur `save apk`

&nbsp;

![69e73643737ad6b4f70d06ef78d2d496.png](../_resources/69e73643737ad6b4f70d06ef78d2d496.png)

Et voila vous avez l'apk sans problème de su

Bien entendu cette solution n'est que temporaire en attendant une mise a jour qui corrige sourcis
