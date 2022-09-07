# DL4NLP
## MetaphorDetection

In this project we use a BERT model to find Metaphors in old german texts. The work is an extension on a project by a [student group from TU Darmstadt](https://github.com/DatNguyen2084/DLDH-Metaphor-detection). We identify the low sample size and extreme class imbalance as main issues. We combat the issues from several angles:

- oversampling by translation (en, da, pl, cs)
- average-precision as meaningful metric
- focal loss as loss function
- an appropriate BERT-variant

Feel free to read throught the project or extend on the work.


## Suggestions for further research:

- check backtranslations to see if they still contain metaphors (use several annotators), and override the copied labels from the german originals
- include french and dutch backtranslations to further increase sample size
- train even more epochs on Focal Loss (So far the hardware accalerated version of Focal Loss was not supported yet, at least on M1 Chips. By the time you work on this you might be able to incorporate hardware support for Focal Loss. So far the training time has been a major bottleneck)
- just repeat experiments, but with different train / test splits, to gain confidence estimates of the Macro F1 scores
- Feel free to reach out with any questions.
