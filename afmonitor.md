Le Monitor est une interface Web qui permet de visualiser les Jobs en cours de calcul

Commandes possible depuis le monitor:
* Mettre en pause un job ou le restart 
* Envoyer des commandes sur les serveurs 
* Redemmarer un ordinateur
* Suspendre un Ordinateur de calcul

!!! Warning
	Le monitor ne permet pas de changer les priority, il faudra les changer depuis la watch

# Interface

web gui [DRACO](https://github.com/Arubinu/Draco-CGRU)


## Command line

!!! Info
	Il est possible d'envoyer un commande a plusieurs serveurs simultanement
	via l'interface web d'afanasy en faisant clique droit sur un serveur 
	puis "launch comand" la commande sera executer sur l'ordinateur en question

***

### Maya
![Maya](img/Software_icon/maya.png){: align=right }
#### Lancer vrayspawner maya 2020
* `cd C:\Program Files\Autodesk\Maya2020\vray\bin && vraymayaspawner2020.exe`

#### Fermer un spawner maya
* `taskkill /f /im vraymayaspawner2015.exe`
* `taskkill /f /im vraymayaspawner2017.exe`
* `taskkill /f /im vraymayaspawner2018.exe`
* `taskkill /f /im vraymayaspawner2019.exe`
* `taskkill /f /im vraymayaspawner2020.exe`
* `taskkill /f /im vray.exe`

***

### 3dsmax
![3dsmax](img/Software_icon/3dsmax.png){: align=right }
#### Lancer vrayspawner 3dsmax 2020
* `cd C:\Program Files\Autodesk\3ds Max 2020\ && vrayspawner2020.exe`

#### Fermer un spawner max
* `taskkill /f /im vrayspawner2020.exe`

#### Ajouter 3dsmax pare feu en TCP et UDP
* `netsh advfirewall firewall add rule name="3dsmax" program="C:\Program Files\Autodesk\3ds Max 2020\3dsmax.exe" dir=in action=allow protocol=tcp profile=public,Private` - TCP
* `netsh advfirewall firewall add rule name="3dsmax" program="C:\Program Files\Autodesk\3ds Max 2020\3dsmax.exe" dir=in action=allow protocol=udp profile=public,Private` - UDP

***

### Blender
![Blender](img/Software_icon/blender.png){: align=right }
#### Installer Blender en ligne de commande
* `msiexec /i "\\10.0.0.203\Sources\01_3D\02_Softwares\Blender\blender-2.83.3-windows64.msi" /qn /norestart`

***

### Lecteur réseaux

* `net use J: \\10.0.0.203\BigCompany\DISNEY_US_Mickey_Mouse_wraps /persistent:yes` - Réactive ou crée un lecteur Réseau 