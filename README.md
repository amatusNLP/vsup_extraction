## Introduzione

La tabella mostra i risultati dell'estrazione automatica di costruzioni a verbo supporto dai corpus [Paisà](https://www.corpusitaliano.it/) e [ItaIst](https://huggingface.co/datasets/VerbACxSS/ItaIst).

L'estrazione delle costruzioni a verbo supporto è stata effettuata confrontando la similarità semantica tra verbi semanticamente pieni e combinazioni di verbo supporto + nome, dove quest'ultimo è morfologicamente correlato al verbo pieno.

## Descrizione dei File:

### VerbiAGGREGATO.xlsx:

contiene tutti i verbi su cui è stata effettuata l’analisi. Le colonne sono 4:
1.	Verbo
2.	Nome
3.	Tipo: (verbo) denominale o (nome) deverbale
4.	Fonte: raccolta delle varie fonti utilizzate. Legenda delle fonti in tab2

### risultatiEstrazione.xlxs:

contiene i risultati divisi su 3 tabs. Le colonne contengono le seguenti informazioni:
1.	struttura analitica (candidato) (lemmatizzato)
2.	verbo sintetico (lemmatizzato)
3.	struttura sintattica
4.	punteggio di similarità (Distributional Semantics)
5.	frequenza Paisà candidato
6.	frequenza Paisà verbo sintetico
7.	frequenza Paisà nome
8.	frequenza Paisà vsup
9.	frequenza ItaIst candidato
10.	frequenza ItaIst verbo sintetico
11.	frequenza ItaIst nome
l2.	frequenza ItaIst vsup
13.	frequenza Low candidato
14.	frequenza Low verbo sintetico
15.	frequenza Low nome
16.	frequenza Low vsup
17.	Pointwise Mutual Information (Paisà)
18.	Rapporto Analitico/Sintetico Paisà
19.	Rapporto Analitico/Sintetico ItaIst

Nel primo tab sono presenti tutte le costruzioni estratte (circa 71 mila).

Il secondo tab (VSUP_RISTRETTO) contiene tutte le costruzioni con i verbi supporto (circa 9000)
1.	Avere
2.	Fare
3.	Dare
4.	Prendere
5.	Mettere

Il terzo tab (ITAIST_PRESENTE) contiene solo le righe del VSUP_RISTRETTO il cui verbo sintetico o analitico appare nel corpus ItaIst almeno una volta

```
@online{VsupItaIst,
  title = {Costruzioni a verbo supporto nell'italiano istituzionale},
  author = {Cirillo, Nicola and Maisto, Alessandro},
  year = {2024},
  url = {[https://github.com/amatusNLP/vsup_extraction]},
  urldate = {2024-11-27}
}
```
