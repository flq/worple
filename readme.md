# Wordle Solver in Picat

## Prerequisites

You should have [picat](https://picat-lang.org) available. Follow the instructions [found on their website](https://picat-lang.org/download.html).


## What does it do?

The script runs in a loop. Based on guess and wordle's feedback, remaining words are evaluated against how much information they're able to extract from the pool of remaining words. The best scoring words are presented to the user. This script is tuned to play wordle **in normal mode**.

## Using it

You can run the script contained like

```bash
picat worlde.pi
```

## Contained words

The word list is taken from Stanford University, original [source here](https://www-cs-faculty.stanford.edu/~knuth/sgb-words.txt).