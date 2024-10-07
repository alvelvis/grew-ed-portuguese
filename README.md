# grew-ed-portuguese
Datasets and rules used in a paper accepted for STIL 2024: Automatic Annotation of Enhanced Universal Dependencies for Brazilian Portuguese

The repository is organized as follows:

- The Grew tool, used to annotate the datasets, was installed from https://grew.fr/usage/install/
- `conjunto_regras_avaliacao.grs` is the file containing modified rules used to evaluate Grew for Portuguese in the annotation of EUD
  - The strategy used for the modified rules was: `strat_modificadas`
- The original rules were obtained from: https://gitlab.inria.fr/grew/udtoeud/-/blob/master/grs/iwpt_UD_to_MIX.grs
  - The strategy used for the original rules was: `ud_to_mix`
- Files that begin with `amostra_` are the samples from Porttinari:
  - `_dev` is the development data without EUD
  - `_test` is the test data without EUD
  - `_gold` is the gold standard EUD annotation for both `_dev` and `_test`
  - `_GREWED` is the automatic EUD annotation by GREW using the original rules
  - `_GREWED-modified` is the automatic EUD annotation by GREW using the modified rules
- `amostra_test_gold.html` and `amostra_dev_gold.html` illustrate the automatic classifications of the enhanced relations in the gold standard among the 6 types of EUD
