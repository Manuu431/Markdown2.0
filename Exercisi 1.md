Exercici GIT 1: Creació i actualització de repositoris
=
Exercici 1
-
1. Crea un repositori nou amb el nom llibre i mostrar el seu contingut.

		mkdir llibre
		cd llibre/
		git init
		ls -la
3. Configura Git definint el nom de l'usuari, el correu electrònic i activar l'exida en color. Mostrar la configuració final.

		git config --global user.name "Manuel Padilla"
		git config --global user.email "manuel@gmail.com"
		git config --global color.ui auto
		git config --list

Exercici 2
-
1. Comprova l'estat del repositori.

		git status
2. Crea un fitxer índex.txt amb el següent contingut:

 		echo "Capítol 1: Introducció a Git" > index.txt
		echo "Capítol 2: Fluxe de treball bàsic >> index.txt
		echo "Capítol 3: Repositoris remots" >> index.txt
3. Comprova de nou l'estat del repositori.

		git status
4. Afegeix el fitxer a la zona d'intercanvi temporal.

		git add index.txt
5. Tornar a comprovar una vegada més l'estat del repositori.

		git status
Exercici 3.
-
Realitza un commit dels últims canvis amb el missatge "Afegit índex del llibre." i veure l'estat del repositori.

	git commit -m "Afegit index del llibre"
	git status
Exercici 4
-
1. Canvia el fitxer índex.txt perquè continga el següent:
Capítol 1: Introducció a Git
Capítol 2: Fluxe de treball bàsic
Capítol 3: Gestió de branques
Capítol 4: Repositoris remots

		nano index.txt
2. Mostra els canvis respecte a l'última versió guardada al repositori.

		git status
3. Fer un commit dels canvis amb el missatge "Afegit capítol 3 sobre gestió de branques".

		git commit -m "Afegit commit capítol 3 sobre gestió de branques"
Exercici 5
-
1. Mostrar els canvis de l'última versió del repositori respecte a l'anterior.

		git diff
2. Canviar el missatge de l'últim commit a "Afegit capítol 3 sobre gestió de branques a l'índex."

		git commit --amend -m "Afegit capítol 3 sobre gestió de branques a l'índex"
3. Tornar a mostrar els últims canvis del repositori.

		git diff
Exercici 6.
-
Indica a Git que vols ignorar tots els fitxers que comencen per "daw", tots els que tenen l'extensió out i les imatges (jpg, png, bmp i gif).
daw*
*.out
*.jpg
*.png
*.bmp
*.gif

	nano .gitignore
