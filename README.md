# DL4NLP
MetaphorDetection

In this project we use a BERT model to find Metaphors in old german texts. The work is an extension on a project by a [student group from TU Darmstadt](https://github.com/DatNguyen2084/DLDH-Metaphor-detection). We identify the low sample size and extreme class imbalance as main issues. We combat the issues from several angles:

- oversampling by translation (en, da, pl, cs)
- average-precision as meaningful metric
- focal loss as loss function
- an appropriate BERT-variant

Feel free to read throught the project or extend on the work
