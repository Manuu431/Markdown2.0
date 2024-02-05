Exercici GIT 2: Ús de l'historial de canvis

Exercici 1

1. Mostra l'historial de canvis del repositori.
2. Crea la carpeta capítols i dins d'ella crea el fitxer capitol1.txt amb el següent text:
   mkdir titols
   cd titols/
   nano capitol1.txt
5. Afegeix els canvis a la zona d'intercanvi temporal (staging area)
   git add capitol.txt
6. Fes un commit dels canvis amb el missatge "Afegit capítol 1."
   git commit -m «Afegit capítol 1.»
7. Torna a mostrar l'historial de canvis del repositori.
           
Exercici 2

1. Crea el fitxer capitol2.txt a la carpeta capítols amb el següent text:
   echo «El flux de treball bàsic amb Git consistexixen:
   1- Fer canvis al repositori.
   2- Afegir els canvis a la zona d’intercanvi temporal.
   3- Fer un commit dels canvis» > capitol2.txt
3. Afegeix els canvis a la zona d'intercanvi temporal.
   Git add capitol2.txt
4. Fes un commit dels canvis amb el missatge "Afegit capítol 2."
   git commit -m «Afegit capítol 2.»
5. Mostra les diferències entre l'última versió i les dues versions anteriors.
      
Exercici 3

1. Crea el fitxer capitol3.txt a la carpeta capítols amb el següent text:
   echo «Git permet la creació de branques, la qual cosa permet tindre distintes versions del mateix projecte i treballar simultàniament en elles» > capitol3.txt   
2. Afegeix els canvis a la zona d'intercanvi temporal.
   Git add capitol3.txt
3. Fes un commit dels canvis amb el missatge "Afegit capítol 3."
   git commit -m "Afegit capítol 3."
4. Mostra les diferències entre la primera i l'última versió del repositori.
       
Exercici 4

1. Afegir al final del fitxer índex.txt la següent línia:
   cd ..
   echo «Capítol 5: Conceptes avançats» > índex.txt
2. Afegir els canvis a la zona d'intercanvi temporal.
   Git add index.txt
3. Fer un commit dels canvis amb el missatge "Afegit capítol 5 a l'índex."
   git commit -m «Afegit capítol 5 a l’índex»
4. Mostrar qui ha fet canvis sobre el fitxer índex.txt.
