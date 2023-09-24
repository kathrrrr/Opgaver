
## Øvelser
Herunder en række øvelser. Som minimum bør man lave 1. til og med 8. Gerne lav et af projekterne. 

1. Forklar hvad funktionen gør og udskriv kaldene for sum(5):
```javascript
function sum(n) {
  if (n == 0 || n == 1)
    return 1;
  if (n > 0)
    return n + sum(n ‐ 1);
}
```
2. Skriv en rekursiv funktion, der beregner eksponenten af et ta.
3. Skriv en funktion der rekursivt skifter mellem at addere og subtrahere tal i en liste. Hvis listen eksempelvis er [5,3,1,2,4] så skal funktionen udregne: 5-3+1-2+4=5.
4. Skriv en rekursiv funktion, der tegner et kvadrat inde i et kvadrat inde i kvadrat indtil den når en vis dybde.
5. Skriv en rekursiv funktion der undersøger om et tal er lige eller ulige
6. Hvad gør følgende funktion. Forklar koden i detaljer:
```javascript
function recBinSearch(n, arr) {
  let mid = Math.floor(arr.length / 2);
  if (arr.length === 1 && arr[0] != n) {
    return false;
  }
  if (n === arr[mid]) {
    return true;
  } else if (n < arr[mid]) {
    return recBinSearch(n, arr.slice(0, mid));
  } else if (n > arr[mid]) {
    return recBinSearch(n, arr.slice(mid));
  }
}
```
7. Skriv en rekursiv funktion, der undersøger om et ord er et palindrome. Dvs. hvorvidt det læses forfra og bagfra på samme måde. 
8. Skriv en rekursiv funktion der tegner en vandret linje, og nedenunder tegner samme vandrette linje, men hvor den miderste tredjedel er væk, fortsæt med at fjerne den miderste tredjedel indtil du har tegnet de første 15 linjer.
9. Skriv en rekursiv funktion, der finder største fælles divisor af to tal
10. Skriv en rekursiv funktion, der returnerer alle tænkelige permutationer af et ord (eksempel: ”abc” så er ”acb” en permutation.
11. Skriv en rekursiv funktion, der beregner mindste fælles divisor
12. Skriv en rekursiv funktion der afgør om et naturligt tal er et primtal eller ej. 
13.  Skriv en rekursiv funktion, der konstruerer og visualiserer Pascals Trekant.	
14. Skriv en rekursiv funktion, der finder det største tal i en liste
15. Skriv en rekursiv funktion, der beregner Tribonacci rækkefølgen  (starter med 0,0,1)
16. Udvid koden for fraktaltræer, så der dannes grønne blade for enden af grenene.


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
