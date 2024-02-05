Exercici GIT 3: Desfer canvis

Exercici 1

1. Elimina l'última línia del fitxer índex.txt i guarda-ho.

		nano index.txt
3. Comprova l'estat del repositori.
4. Desfés els canvis realitzats al fitxer índex.txt per tornar a la versió anterior del fitxer.

		git checkout – index.txt
6. Torna a comprovar l'estat del repositori.

Exercici 2

1. Elimina l'última línia del fitxer índex.txt i guarda-ho.

		nano index.txt
2. Afegeix els canvis a la zona d'intercanvi temporal.

		git add index.txt
4. Comprova de nou l'estat del repositori.
5. Treu els canvis de la zona d'intercanvi temporal, però mantin-los al directori de treball.

		git reset --soft HEAD
7. Comprova de nou l'estat del repositori.
8. Desfés els canvis realitzats al fitxer índex.txt per tornar a la versió anterior del fitxer.

		git checkout – index.txt
10. Torna a comprovar l'estat del repositori.

Exercici 3

1. Elimina l'última línia del fitxer índex.txt i guardar-ho.
2. Elimina el fitxer capítols/capitol3.txt.

		cd titols/
		rm capitol3.txt
4. Afegeix un fitxer nou capítols/capitol4.txt buit.

		nano capitol4.txt
6. Afegeix els canvis a la zona d'intercanvi temporal.

		git add capitol4.txt
8. Comprova de nou l'estat del repositori.
9. Treu els canvis de la zona d'intercanvi temporal, però mantin-los al directori de treball.

		git reset --soft HEAD
11. Comprova de nou l'estat del repositori.
12. Desfés els canvis realitzats per tornar a la versió del repositori.
  
		git reset –hard HEAD
13. Torna a comprovar l'estat del repositori.
       
Exercici 4

1. Elimina l'última línia del fitxer índex.txt i guardar-ho.
2. Elimina el fitxer capítols/capitol3.txt.

		cd titols/
		rm capitol3.txt
4. Afegeix els canvis a la zona d'intercanvi temporal i fer un commit amb el missatge "Borrat accidental."

		git add .
   git commit -m «Borrat accidental»
6. Comprova l'historial del repositori.

		git log
7. Desfés l'últim commit, però mantin els canvis anteriors al directori de treball i a la zona d'intercanvi temporal.

		git reset –soft HEAD
8. Comprova l'historial i l'estat del repositori.
9. Torna a fer el commit amb el mateix missatge d'abans.
10. Desfés l'últim commit i els canvis anteriors al directori de treball, tornant a la versió anterior del repositori.

		git reset –soft HEAD
11. Comprova de nou l'historial i l'estat del repositori.
