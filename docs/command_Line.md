# Command line utile:

## Maya
![Maya](img/blender.png)
### Lancer vrayspawner maya 2020
* `cd C:\Program Files\Autodesk\Maya2020\vray\bin && vraymayaspawner2020.exe`

### Fermer un spawner maya
* `taskkill /f /im vraymayaspawner2015.exe`
* `taskkill /f /im vraymayaspawner2017.exe`
* `taskkill /f /im vraymayaspawner2018.exe`
* `taskkill /f /im vraymayaspawner2019.exe`
* `taskkill /f /im vraymayaspawner2020.exe`
* `taskkill /f /im vray.exe`

***

## 3dsmax

### Lancer vrayspawner 3dsmax 2020
* `cd C:\Program Files\Autodesk\3ds Max 2020\ && vrayspawner2020.exe`

### Fermer un spawner max
* `taskkill /f /im vrayspawner2020.exe`

***

### Ajouter 3dsmax pare feu en TCP et UDP
* `netsh advfirewall firewall add rule name="3dsmax" program="C:\Program Files\Autodesk\3ds Max 2020\3dsmax.exe" dir=in action=allow protocol=tcp profile=public,Private` - TCP
* `netsh advfirewall firewall add rule name="3dsmax" program="C:\Program Files\Autodesk\3ds Max 2020\3dsmax.exe" dir=in action=allow protocol=udp profile=public,Private` - UDP

## Blender

### Installer Blender en ligne de commande
* `msiexec /i "\\10.0.0.203\Sources\01_3D\02_Softwares\Blender\blender-2.83.3-windows64.msi" /qn /norestart`