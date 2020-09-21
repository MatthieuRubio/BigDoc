# Pré-requis
* Python
* Mkdocs 

!!! Info
	Pour installer Mkdocs ouvrir un invite de commande et éxécuter  la commande  
	`pip install mkdocs`

# Modification

 * copier le dossier "BigDocumentation "\\\\10.0.0.203\Sources\01_3D\02_Softwares\CGRU\\_Documentation\" sur le disque C:
 * Pour visualiser les modification en live ouvrir un invite de commande et executer la commande `cd c:\BigDocumentation && mkdocs serve` ou executer le fichier `Serveur.bat` qui se trouve dans C:\BigDocumentation
 * Rendez vous ensuite sur votre navigateur internet a l'adresse `http://127.0.0.1:8000/` c'est l'adresse qui vous permettra de visualiser les modification effectuer en local
 
### Créer une nouvelle page:

1. Créer un nouveau fichier nommé "nomdelapage.md" dans le dossier   
"C:\BigDocumentation\docs"
2. Ouvrir le fichier **mkdocs.yml** qui se trouve dans le dossier "C:\BigDocumentation" avec votre éditeur de texte
3. Ajouter une ligne Pour créer le lien entre le fichier .md et mkdocs  
	`- Nom de la page: nomdelapage.md` - Nomenclature de la ligne : "Nom de la page" sera le texte afficher dans le menu et "nomdelapage.md" correspond au fichier present dans votre dossier  

	#### exemple:

			nav:									
				- Home: index.md
				- Page01: page01.md
				- Page02: page02.md
				- Nom de la page: nomdelapage.md  //ici la page sera inséré apres la page 02
			...
				
	!!! Info
		L'emplacement de cette ligne correspondra a son emplacement dans le menu a gauche

*** 

# Publier sur le site web

Le site web est hebergé sur la 192.168.1.200 avec un serveur wamp

!!! Info
	Pour Publier automatiquement la mise a jour de la documentation, executer le fichier "AutoBuild_doc_and_publish.bat" qui se trouve a la racine du dossier "C:\BigDocumentation"
	(ce fichier execute la commande `mkdocs build` et copie ensuite le dossier site dans le dossier  "\\\\192.168.1.200\BigDocumentation"

!!! Warning
	Si l'update ne s'est pas faite correctement, essayer de supprimer le contenu du dossier \\\\192.168.1.200\BigDocumentation avant d'executer le fichier "AutoBuild_doc_and_publish.bat"

### Publier le site manuellement
1. Supprimer le dossier "Site" qui se trouve dans C:\BigDocumentation si il existe
2. Dans un invite de command executer la commande `cd c:\BigDocumentation && mkdocs build` 
3. Copier le dossier site qui viens d'être crée dans C:\BigDocumentation Dans le dossier suivant : "\\\\192.168.1.200\BigDocumentation"



# Mkdocs help

For full documentation visit [mkdocs.org](https://www.mkdocs.org).

## Commands


## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.

# Wamp server

!!! Info
	[Erreur partage du site sur le reseau local](https://www.johannesrabeyrin.fr/wamp-corriger-forbidden-you-dont-have-permission-to-access-on-this-server/)


# Exemples markdown

---
```
> **_NOTE:_**  The note content.
```
> **_NOTE:_**  The note content.
***
```
[![Ask Me Anything !](https://img.shields.io/badge/%20Jobs-Done-1abc9c.svg)](https://GitHub.com/Naereen/ama)
```
[![Ask Me Anything !](https://img.shields.io/badge/%20Jobs-Done-1abc9c.svg)](https://GitHub.com/Naereen/ama)
***
```
!!! Tip
	text
```
!!! Tip
	text
***
```
!!! Info
	text
```
	
!!! Info
	text
***
```
!!! Warning
	text
```	
!!! Warning
	text
***
```	
!!! Danger
	text
```		
!!! Danger
	text
***

| Method      | Description                          |
| ----------- | ------------------------------------ |
| `GET`       | test  |
| `PUT`       | test |
| `DELETE`    | test |



    int main()
    {
        printf("Hello world!\n");
        return 0;
    }