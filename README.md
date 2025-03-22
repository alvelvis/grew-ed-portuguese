# grew-ed-portuguese
Datasets and rules used in a paper accepted for STIL 2024: Automatic Annotation of Enhanced Universal Dependencies for Brazilian Portuguese

The repository is organized as follows:

- The Grew tool, used to annotate the datasets, was installed from https://grew.fr/usage/install/
- `conjunto_regras_avaliacao.grs` is the file containing modified rules used to evaluate Grew for Portuguese in the annotation of EUD
  - The strategy used for the modified rules was: `strat_modificadas`
  - This file did not change since the publicaton of the conference paper: https://sol.sbc.org.br/index.php/stil/article/view/31134
  - However, we have updated the rules to increase its accuracy afterwards, generating the `conjunto_regras_porttinari.grs`, which is also the rules used to annotate the whole Porttinari corpus. This set of rules can be found at https://github.com/alvelvis/eud-portugues. The current version of .conllu files are annotated using the most recent rules.
- The original rules were obtained from: https://gitlab.inria.fr/grew/udtoeud/-/blob/master/grs/iwpt_UD_to_MIX.grs
  - The strategy used for the original rules was: `ud_to_mix`
- Files that begin with `amostra_` are the samples from Porttinari:
  - `_dev` is the development data without EUD
  - `_test` is the test data without EUD
  - `_gold` is the gold standard EUD annotation for both `_dev` and `_test`
  - `_GREWED` is the automatic EUD annotation by GREW using the original rules
  - `_GREWED-modified` is the automatic EUD annotation by GREW using the modified rules
- `amostra_test_gold.html` and `amostra_dev_gold.html` illustrate the automatic classifications of the enhanced relations in the gold standard among the 6 types of EUD
- `divergencias_` files show the divergences between gold and automatic annnotation

# Changelog

- 2025-03-19 - a few changes have been made to the datasets and the rules to increase its accuracy
