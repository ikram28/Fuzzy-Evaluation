# Fuzzy Inference System for Internship Report Evaluation 

This project aims to implement a Mamdani-type fuzzy inference system for evaluating internship reports using the Python Fuzzy-Expert package. The fuzzy system takes three input variables: 
- Results Obtained (out of 20),
- Methods Used (out of 20),
- Presentation (out of 20).
- 
It outputs the overall evaluation of the report on a scale of 20.

For each input variable, three linguistic values are defined: **Poor, Average, Excellent**.

However, for the overall evaluation, five linguistic values are defined: **Poor, Bad, Average, Good, Excellent**.

## Rule Base

The rule base consists of the following six rules:

- Rule 1 (R1): If Result is Average AND Methods is Poor THEN Evaluation is Bad
- Rule 2 (R2): If Result is Average AND Methods is Excellent THEN Evaluation is Good
- Rule 3 (R3): If Result is Poor AND Methods is Average THEN Evaluation is Bad
- Rule 4 (R4): If Result is Excellent AND Methods is Excellent AND Presentation is Excellent THEN Evaluation is Excellent
- Rule 5 (R5): If Result is Poor OR Methods is Average THEN Evaluation is Average
- Rule 6 (R6): If Result is Average OR Methods is Poor THEN Evaluation is Poor
