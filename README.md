<img src="logo.svg" alt="ChemTrain logo" height="110" align="right">

# Chirality Learn

Chirality Learn is a Quizlet-style trainer for assigning stereochemistry by the Cahn–Ingold–Prelog (CIP) priority rules: R/S at stereocentres, E/Z at double bonds and Re/Si at prochiral faces, on drugs, metabolites and natural products. Everything is in one HTML file.

**Play it here:** https://chemtrain.github.io/chirality-learn/chirality_learn.html

You can also download `chirality_learn.html` and open it in any browser.

## What's inside

- 101 molecules in eight sets: first stereocentres, single-enantiomer drugs (chiral switches), several stereocentres (β-lactams, statins, antivirals), steroids and polycycles, tricky priorities (L-cysteine is R), sulfur and phosphorus centres (esomeprazole, sofosbuvir), E/Z double bonds (tamoxifen, retinoids, oximes) and Re/Si faces (pyruvate, acetophenone, drug intermediates)
- 164 stereocentres, 30 stereogenic double bonds and 10 prochiral carbonyls
- Six kinds of question, each one a toggle: R/S at a marked stereocentre, E/Z at a marked double bond, Re/Si for the face toward you, ranking lettered groups by priority, assigning every centre of a molecule at once, and counting the stereocentres of a structure drawn without wedges
- A worked answer to every question: the groups numbered by priority on the drawing, why each beats the next (the sets of atoms compared, sphere by sphere, duplicate atoms in brackets), and how the label follows from where the lowest group points
- H at the stereocentres drawn on a wedge or hash, or implied as on a drug label
- A note on every molecule: why its stereochemistry matters, with links to Wikipedia and PubChem
- Learn mode, flashcards, a card list, and My cards for the ones you star

## How the answers are checked

The structures are PubChem's. For every molecule, the build checks that

1. the stereodescriptors RDKit's CIP labeller assigns (2013 IUPAC rules) are the ones typed from the literature, and those in PubChem's IUPAC name;
2. its own CIP ranking of the groups (a breadth-first hierarchical digraph, the way a student works it out), applied to the 2D drawing on the page with its wedges and hashes, gives the same label for every stereocentre, double bond and face, in every drawing;
3. for a prochiral carbonyl, the face read from the drawing agrees with RDKit's label of the alcohol made by adding hydride from the front.

## Sources

Structures from [PubChem](https://pubchem.ncbi.nlm.nih.gov/). Labels follow the IUPAC 2013 recommendations (P-92) as implemented in RDKit ([Hanson et al., *J. Chem. Inf. Model.* 2018, 58, 1755](https://doi.org/10.1021/acs.jcim.8b00324)). Notes on each molecule are from its Wikipedia article unless they cite another source. Structures are drawn with [RDKit](https://www.rdkit.org).

## How to cite

If you use Chirality Learn in a course, a worksheet or a paper, please cite it:

> Brandon, L. *Chirality Learn* (2026). ChemTrain. https://github.com/ChemTrain/chirality-learn

GitHub's **Cite this repository** button (from `CITATION.cff`) gives the same reference in APA and BibTeX.

## License

- Code (the HTML, CSS and JavaScript): [MIT](LICENSE).
- Content (the cards, questions, notes and structure drawings): [CC BY 4.0](LICENSE-CONTENT.md). You may reuse and adapt it, as long as you credit Chirality Learn.
- Logo (`logo.svg`): the locomotive is adapted from [Twemoji](https://github.com/jdecked/twemoji), © Twitter, Inc and other contributors, licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/); the benzene-ring smoke was added for ChemTrain.
