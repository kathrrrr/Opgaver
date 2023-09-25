
## Øvelser
Øvelserne er taget fra Henrik Sterners p5js opgaver og ændret til python
Herunder en række øvelser. Som minimum bør man lave 1. til og med 8. Gerne lav et af projekterne. 

1. Forklar hvad funktionen gør og udskriv kaldene for sum(5):
```python
def sum(n):
    if n == 0 or n == 1 :
        return 1
    if n > 1 :
        return n + sum(n-1)
    
```
2. Skriv en rekursiv funktion, der beregner eksponenten af et tal.
3. Skriv en funktion der rekursivt skifter mellem at addere og subtrahere tal i en liste. Hvis listen eksempelvis er [5,3,1,2,4] så skal funktionen udregne: 5-3+1-2+4=5.
4. Skriv en rekursiv funktion der undersøger om et tal er lige eller ulige
5. Hvad gør følgende funktion. Forklar koden i detaljer:
```python
import math

def binSearch(n, arr) :
    mid = math.floor(len(arr) / 2)
    if len(arr) == 1 and arr[0] != n : 
        return False
  
    if n == arr[mid] :
        return True
    elif n < arr[mid] :
        return binSearch(n, arr[0: mid])
    elif n > arr[mid] :
        return binSearch(n, arr[mid:len(arr)-1])

```
6. Skriv en rekursiv funktion, der undersøger om et ord er et palindrome. Dvs. hvorvidt det læses forfra og bagfra på samme måde. 
7. Skriv en rekursiv funktion, der finder største fælles divisor af to tal
8. Skriv en rekursiv funktion, der returnerer alle tænkelige permutationer af et ord (eksempel: ”abc” så er ”acb” en permutation.
9. Skriv en rekursiv funktion, der beregner mindste fælles divisor
10. Skriv en rekursiv funktion der afgør om et naturligt tal er et primtal eller ej. 
11.  Skriv en rekursiv funktion, der konstruerer Pascals Trekant.	
12. Skriv en rekursiv funktion, der finder det største tal i en liste
13. Skriv en rekursiv funktion, der beregner Tribonacci rækkefølgen  (starter med 0,0,1)



## Projekt: Selv-similære figurer
I følgende projekt skal du implementere visuelle repræsentationer af forskellige selv-similære figurer. Dvs. figurer hvor et vilkårligt udsnit af figuren ligner helheden af den samlede figur.

### Konstruer en visuel repræsentation af Cantors mængde
Cantors mængde er opkaldt efter den tyske matematiker Georg Cantor.

Det er en relativt simpel konstruktion, hvor man tager udgangspunkt i et linjestykke. Del stykket ind i tre mindre dele og fjern det miderste stykke. Fortsæt herefter på tilsvarende vis med de de resterende stykker. 

### Konstruer en visuel repræsentation af Kochs snefnugskurve
I Kochs snefnugskure der tredeles ethvert linjestykke i tre lige store dele. Den miderste del fjernes og erstattes af to sider i den ligesidede trekant. Processen gentages på hvert af de nye linjestykker. 

Kochs snefnugskurve er et eksempel på en fraktal


### Konstruer en visuel repræsentation af Sierpinskis trekant

Herunder beskrives konstruktion i prosakode. Dvs. tekst der er mere eller mindre kodenær:

1. Start med at konstruere en ligesidet trekant. Dvs. en trekant hvor alle sider er lige lange (og vinkler lige store).

2. Inddel trekanten i fire kongruente og ligesidede trekanter ved at bestemme midtpunkter for de tre sider i den oprindelige trekant.

3. Fjern den miderste trekant.

4. Gentag trin 2 og 3 for de tre resterende trekanter.
