# Wordle Solver in Picat

## Prerequisites

You should have [picat](https://picat-lang.org) available. Follow the instructions [found on their website](https://picat-lang.org/download.html).


## What does it do?

The script runs in a loop. Starting with the best start against the provided dictionary (TARES), the script expects you to enter the guesses result. The next guess is evaluated against how much information they're able to extract from the pool of remaining words. The one scoring best in terms of entropy decrease will be shown to the user, repeating the loop. This script is tuned to play wordle **in normal mode**.

## Using it

You can run the script contained like

```bash
picat worlde.pi
```

## Elephant memory mode

Assuming wordle doesn't play out a previous word again, a list containing most of the played words so far is included. In order to use it, run

```bash
picat wordle.pi use-played
```

## Contained words

The word list is taken from Stanford University, original [source here](https://www-cs-faculty.stanford.edu/~knuth/sgb-words.txt).