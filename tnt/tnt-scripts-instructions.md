# TNT Scripts Instructions
---

*Disclaimer*: The scripts provided here were written by Laura Rocha Prado, following guidelines described by TNT authors. They have been tested only in Windows environments. Please read the contents of the script to understand what's going on step-by-step (each command has been commented for clarity).

## Usage

1. Make sure you have extracted the TNT scripts that are shipped with it (tnt_scripts.zip) to the root folder. My scripts need to call other TNT scripts during their run, so they will not work if this step isn't completed.
2. Add both your matrix and the desired script to your root folder (i. e., the folder where TNT is installed).
3. Start TNT, and turn macros on before you do anything. Do this via menu, by clicking option Settings -> Enable macros; or, via command line, typing `macro=` and pressing Enter.
4. Open your matrix file.
5. Via command line, type `run scriptname`, where `scriptname` should be replaced by the exact name of the script file.

## Available scripts

- `TBRequalweights.run`: This script will run a traditional search (RAS+TBR) with 10000 replicates, holding 10 trees per replicate, with memory available for 100.000 trees. Collapsing is off. If there are multiple trees found, a consensus tree will be produced.Tree files will be generated, in both notations (compact and parenthetical), with general tree file including consensus tree as the last one.
- `TBRimpliedweighting.run`: This script will run a traditional search (RAS+TBR) with 10000 replicates, holding 10 trees per replicate, with memory available for 100.000 trees. Collapsing is off. `Piwe` should already be set with the desired `k` value. If there are multiple trees found, a consensus tree will be produced. Tree files will be generated, in both notations (compact and parenthetical), with general tree file including consensus tree as the last one.