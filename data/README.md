# Explanation

The data reside in two CSV files which are merged and preprocessed by our analysis scripts:

* `rsos181274supp2.csv`: the original dataset from Koplenig (2019), downloaded on 2 April 2022 from https://royalsocietypublishing.org/doi/suppl/10.1098/rsos.181274 and converted to CSV.
* `koplenig-reply.csv`: our additions.

We add the following columns:

* `ethnologue_L2_users`: boolean. `TRUE` if Ethnologue gives a *numerical* estimate of L2 users for the language (within the "Population" field), `FALSE` otherwise.
* `used_as_L2_by`: character. If Ethnologue states that the language is used as an L2 by some set of languages (within the "Language Use" field; regardless of whether or not it gives a numerical L2 users estimate), this column gives those languages' ISO codes as a colon-separated string. Otherwise, the value is `NA`.
* `notes`: character. Additional notes.

For the meaning of the remaining columns, which are taken from Koplenig's original dataset, we refer the reader to Koplenig's paper.

Like Koplenig, we have used the 20th edition of Ethnologue (2017).
