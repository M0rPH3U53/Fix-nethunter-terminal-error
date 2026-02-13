## ❌ Problème

nhterm: **2025.4** (2025110400)

Magisk: **30.6**

Le problème au démarrage de `nhterm` est qu’il ne trouve pas de binaire `SU`

```
[android-su][ERROR] 'su' binary not found in path 
```

## ✅ Fix & compile 

APK Editor Studio: https://qwertycube.com/apk-editor-studio/download/  
APK d'origine: https://store.nethunter.com/repo/com.offsec.nhterm_2025110400.apk

Apres avoir ouvert l'apk avec **APK Editor Studio** remplacer `/bin/su` par `/bin/bash` dans le fichier kali & enregistrer via **CTRL-S**

<img width="908" height="458" alt="2b41a08788805d3e18ef2943521f3ea0" src="https://github.com/user-attachments/assets/fae35ec1-dee0-42b8-8848-92222c93e5f3" />


&nbsp;

Ensuite aller dans `android-su` et supprimer les " " de “\${SU2\[@\]}” & enregistrer via **CTRL-S**

<img width="850" height="440" alt="23fb925e9afd2384273e7d82c59c24e7" src="https://github.com/user-attachments/assets/758f591c-62bf-40f0-9c57-8a1c93c78848" />


&nbsp;

Fermer les 2 fenêtres des fichier et cliquer sur `save apk`

<img width="1380" height="625" alt="69e73643737ad6b4f70d06ef78d2d496" src="https://github.com/user-attachments/assets/edd7c44b-96d3-44d3-91fb-0a8a1680bdfd" />
&nbsp;

## #️⃣ Nhterm
Dssinstaller la version actuelle et installer votre apk

Donner les droit root via l'app Magisk si celle ci ne pop pas

<img width="524" height="438" alt="magisk" src="https://github.com/user-attachments/assets/e55ffd08-6076-4341-95a8-3c21b1e51b1b" />

&nbsp;

Retablir le shell d'origine  `Settings/Generale Settings/Initial Commande` et mettre  `source /home/kali/.bashrc`

<img width="433" height="426" alt="nhterm" src="https://github.com/user-attachments/assets/6168cf7b-e738-4b88-b477-2b79ff23e973" />

&nbsp;

Shell d'origine

<img width="431" height="108" alt="Capture du 2026-02-12 16-12-37" src="https://github.com/user-attachments/assets/20d69b92-bf87-4e70-9a6b-36edea41d981" />

&nbsp;

⚠️ Bien entendu cette solution n'est que temporaire en attendant une mise a jour qui corrige le sourcis
