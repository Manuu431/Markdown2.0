Exercici GIT 2: Ús de l'historial de canvis
=
Exercici 1
-
1. Mostra l'historial de canvis del repositori.

		git log
2. Crea la carpeta capítols i dins d'ella crea el fitxer capitol1.txt amb el següent text:
Git és un sistema de control de versions ideat per Linus Torvald.

		mkdir titols
		cd titols/
		nano capitol1.txt
3. Afegeix els canvis a la zona d'intercanvi temporal (staging area)

		git add capitol.txt
4. Fes un commit dels canvis amb el missatge "Afegit capítol 1."

		git commit -m «Afegit capítol 1.»
5. Torna a mostrar l'historial de canvis del repositori.

		git log
Exercici 2
-
1. Crea el fitxer capitol2.txt a la carpeta capítols amb el següent text:

		echo «El flux de treball bàsic amb Git consistexixen:
	1.1. Fer canvis al repositori.
	1.2. Afegir els canvis a la zona d’intercanvi temporal.
	1.3. Fer un commit dels canvis» > capitol2.txt
2. Afegeix els canvis a la zona d'intercanvi temporal.

		git add capitol2.txt
3. Fes un commit dels canvis amb el missatge "Afegit capítol 2."

		git commit -m «Afegit capítol 2.»
4. Mostra les diferències entre l'última versió i les dues versions anteriors.

		git diff HEAD~1
		git diff HEAD~2 HEAD~1
Exercici 3
-
1. Crea el fitxer capitol3.txt a la carpeta capítols amb el següent text:

		echo «Git permet la creació de branques, la qual cosa permet tindre distintes versions del mateix projecte i treballar simultàniament en elles» > capitol3.txt   
2. Afegeix els canvis a la zona d'intercanvi temporal.

		git add capitol3.txt
3. Fes un commit dels canvis amb el missatge "Afegit capítol 3."

		git commit -m "Afegit capítol 3."
4. Mostra les diferències entre la primera i l'última versió del repositori.

		git diff HEAD~2 HEAD
Exercici 4
-
1. Afegir al final del fitxer índex.txt la següent línia:

		cd ..
		echo «Capítol 5: Conceptes avançats» > índex.txt
2. Afegir els canvis a la zona d'intercanvi temporal.

		git add index.txt
3. Fer un commit dels canvis amb el missatge "Afegit capítol 5 a l'índex."

		git commit -m «Afegit capítol 5 a l’índex»
4. Mostrar qui ha fet canvis sobre el fitxer índex.txt.

		git blame index.txt
