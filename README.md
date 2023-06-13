# calculator-java
simple calculator written in Java; supports addition, subtraction, multiplication and division
-LOC za kompletan projekat, odnosno za sve fajlove zajedno je 186.
-Ciklomatska složenost- koristeći Codalyze alat u okviru Visal Studio Code dobijeni su podaci:
metoda evaluateExtpresion- ova metoda se nalazi na 28 liniji koda i je do 72 linije koda,
ciklomatska kompleksnost ove metode je 12, ima 33 linije koda i ima 1 parametar.
metoda Calculate- ova metoda se nalazi na 74 liniji koda i do 186 linije koda, 
ciklomatska kompleksnost je 12, ima 77 linija koda i ima 2 parametra.
-Kognitivna složenost kao i u većini slučajeva i ovde je slična ciklomatskoj složenosti. Na osnovu analize ove dve metode, posmatrajući prve if blokove 
i if blokove unutar njih kao i naredne nivoe gnežđenja dobijena je kompleksna složenost za metodu evaluateExtpresion 11, a metoda Calculate 15. 
-Analiza je izvršena Sonarlont alatom u okviru Visual Studio Code i pokazala nam je da postoji 7 problema:
1. Java:S1118 na liniji 4, Code Smell Major
   Add private constructor to hide the implicit public one. 
   SonarLint Rule Description: Utility classes should not have public constructors.
2. Java:S1220 na liniji 1 Code Smell Minor
   Move this file to a named package.
   SonarLint Rule Description: The default unnamed package should not be used.
3. Java:S100 na liniji 18 Code Smell Minor
    Rename this metod name to match the regular expresion '^[a-z][a-zA-ZO-9]*$' 
    SonarLint Rule Description: Method names should comply with a naming convention.
 4. Java:S100 na liniji 24 Code Smell Minor
    Rename this metod name to match the regular expresion '^[a-z][a-zA-ZO-9]*$' 
    SonarLint Rule Description: Method names should comply with a naming convention.
 5. Java:S1488 na liniji 70 Code Smell Minor
     Immediately return this expression instead of assigning in to the temporary variable "textResult".
     SonarLint Rule Description: Local variables should not be declared and then immediately return or thrown. 
 6. Java:S100 na liniji 74 Code Smell Minor
     Rename this metod name to match the regular expresion '^[a-z][a-zA-ZO-9]*$' 
     SonarLint Rule Description: Method names should comply with a naming convention.
 7. Java:S3626 na liniji 183 Code Smell Minor
     Remove this redundant jump.
     SonarLint Rule Description: Jump statements should not be redudant.
     
     Posmatrajući ceo fajl statičkom analizom se može reći da je umereno kompleksan kod, bez puno većih grešaka, tri greške od ukupno sedam su ukazivale 
     na problem naziva same metode. Code Smell je samo na jednom mestu označen kao Major, dok su svi ostali Minor. 
