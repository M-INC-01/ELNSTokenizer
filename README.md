# ELNSTokenizer

Questo repository contiene **ELNSTokenizer**, un tokenizer sviluppato per l’elaborazione del linguaggio naturale in italiano, progettato per essere leggero, efficiente e facilmente integrabile in modelli linguistici personalizzati.

## Contenuti del repository

- 📂 **ELNSTokenizer/**  
  Cartella contenente i file necessari al funzionamento del tokenizer (vocabolario, merges, configurazioni, ecc.).

- 📄 **ELNSTokenizer_WhitePaper.pdf**  
  Documento tecnico (white paper) che descrive nel dettaglio l’architettura, le metodologie di addestramento, i dataset utilizzati e le potenziali applicazioni del tokenizer.  
  Questo documento è pensato per la consultazione scientifica e per una possibile pubblicazione su arXiv.

## Come usare ELNSTokenizer

L’integrazione avviene in maniera analoga ai tokenizer standard di Hugging Face.  
Esempio d’uso (in Python):

```python
from tokenizers import Tokenizer

# Caricamento del tokenizer
tokenizer = Tokenizer.from_file("ELNSTokenizer/tokenizer.json")

# Tokenizzazione di un testo
output = tokenizer.encode("Ciao, questo è un test del tokenizer ELNS.")
print(output.tokens)
```

## Obiettivi

Supportare la lingua italiana in modo nativo e ottimizzato.

Offrire un’alternativa leggera e personalizzabile ai tokenizer generici.

Consentire l’uso in scenari accademici, di ricerca e industriali.


## Licenza

Questo progetto è distribuito con licenza GPLv3.
