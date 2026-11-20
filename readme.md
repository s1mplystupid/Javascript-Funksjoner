# Funksjoner

Oppgavene står i `oppgaver.js`. Skriv koden der det står `// LØSNING`, og kjør fila ofte:

```
node oppgaver.js
```

Sjekken nederst viser `OK` eller `FEIL` for hver oppgave. Hvis du modifiserer oppgaven med andre verdier vil ikke dette fungere. Dette er ok, husk at du legger inn en kommentar som beskriver det.

## Funksjoner

En funksjon tar inn verdier (parametre) og sender et svar ut med `return`. Her har vi laget en funksjon som heter "pluss", og vi sender inn parameterene a og b. I selve funksjonen legger vi sammen tallverdiene. Retur gir derfor sum av inn-verdiene. 

```js
function pluss(a, b) {
  return a + b;
}

pluss(2, 3);   // 5
```

Uten `return` får du `undefined`, og sjekken viser `FEIL`.

**Gjenbruk** betyr at én funksjon kaller en annen:

```js
function dobbel(tall) {
  return tall * 2;
}

function firedobbel(tall) {
  return dobbel(dobbel(tall));
}
```

**Løkke gjennom en array:**

```js
for (let i = 0; i < tall.length; i++) {
  // tall[i] er tallet du står på nå
}
```


## Hint

| Oppgave | Hint |
|---|---|
| 1 | `` return `Hei, ${navn}!`; `` |
| 4 | `let total = 0;` før løkka, `return total;` etter løkka. |
| 7 | Start med `tall[0]`, ikke 0. |
| 8 | `const kalde = [];` og `kalde.push(tall[i]);` |
| 9 | Kopier først: `const kopi = [...tall];`. Bytt to naboer med en `tmp`-variabel. |
| 11 | `return alder >= grense;` gir `true` eller `false`. |
| 13 | Andel = antall i valgt fraksjon / (alliance + horde) * 100. Over 50 gir feilmelding. |
| 15 | `erGammelNok(alder, aldersgrenser[spill])` |
| 16 | Som `sum()`, men legg til `billettpris(deltakere[i].vg1)`. |
| 17 | Som oppgave 9, men sammenlign `.poeng` og sorter fra størst til minst. |

## Dokumentasjon 


```markdown
## kanDelta(alder, spill)
Sjekker om deltakeren er gammel nok til spillet.
Inn: alder (tall), spill (tekst)
Ut: true eller false
Eksempel: kanDelta(16, "GTA 6") -> false
```

Fyll ut egenvurderingen nederst i `oppgaver.js`. Husk commit og push.

## Vurderingsmatrise

| Kriterium | Lav | Middels | Høy |
|---|---|---|---|
| Funksjoner og return | Enkle funksjoner med hjelp | Grønne oppgaver på egen hånd | Funksjoner med arrays og objekter |
| Løkker og arrays | Løkke etter eksempel | Summere og telle (gule oppgaver) | Nye arrays og egen sortering (røde oppgaver) |
| Valg og logikk | Enkel `if` | `if/else` med tekst og prosent | Håndterer grensetilfeller |
| Gjenbruk | Skriver koden på nytt | Gjenbruker når oppgaven sier det | Gjenbruker på eget initiativ |
| Dokumentasjon | Én funksjon kort | Alle funksjonene i del 3 | Så tydelig at andre kan bruke dem |
| Egenvurdering | Noen punkter | Alle punktene | Begrunnet med eksempler fra egen kode |

Innsats og forståelse teller mer enn at alt er perfekt.

