# A practical guide towards explainability and bias evaluation in machine learning

https://pydata.org/london2019/schedule/presentation/1/
https://github.com/EthicalML
https://github.com/EthicalML/explainability-and-bias


Need to consider how "what is right" is not universal. Acceptable behaviour or societal standards might change across from location to location.


explainability != interpretability
- goes beyond the algorithm


Discusses the library: https://github.com/EthicalML/XAI
- mainly a one stop shop for visualising data & model results by variables
- Doesn't appear to dig below the surface, eg nothing about proxies etc



Counterfactual Explanations
- https://docs.seldon.io/projects/alibi/en/stable/methods/CF.html
- What are the minimum changes required to (significantly) change the result, eg turn a 7 into a 9
- Could be good to test errors & how to move through threshold curve & ultimately potentially generate new features
    - eg, this is a bad customer. There are the changes required to make them good
    - Possibly a non-linear alternative to risk scores




Seldon - "enterprise ML deployment platform"
- https://www.seldon.io/


Can deploy a live "explainer" to monitor models in prod



"Smile curves"
- accuracy across the threshold ranges
- colour code by group, TP/FP, etc
- another "one click tool"