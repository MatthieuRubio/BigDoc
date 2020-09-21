# Installation CGRU (Afanasy)

1. Copier le dossier pipeline sur le C:
* Installer [python-3.6.6](https://www.python.org/ftp/python/3.6.6/python-3.6.6.exe)  
(Penser a cocher la case add to path lors de l'installation de python) 
* `python -m pip install --upgrade pip` - Dans un Invite de commande mettre a jour pip
* `python -m pip install PyQt5` - Installer PyQt5
* Installer [Git](https://git-scm.com/download/win)
* `pip install git+https://github.com/Arubinu/jeanpaulstart.git` installer jeanpaulstart

## Lancement De JPS

* se rendre dans le dossier C:\Pipeline et lancer le start_bigmenu.bat
* cliquer sur l'icone Big Company dans le "systeme tray"

!!! Info
	Le "systeme tray" est la zone dans le petite fleche en bas a droite de votre écran

## Configuration du lancement au démarrage

* Copier les fichiers suivant (\\10.0.0.203\Sources\01_3D\02_Softwares\CGRU\startup)
	* “launch_render_startup.bat”
	* “Launch_bat_invisible.vbs”  	 
Dans le dossier suivant:  
(%appdata%\Microsoft\Windows\Start Menu\Programs\Startup)

***