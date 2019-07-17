# The unreasonable effectiveness of feature hashing

https://pydata.org/london2019/schedule/presentation/48/
https://github.com/gcampanella/pydata-london-2019


## Background
- Tackling the problem of high dimentional datasets, eg one-hot encoded text
    - Breaks GLMs
- NN's work best with non-sparse data


## Hashing
- feature value -> hashing fn -> mod(n) to shrink number down
    - Then can use via one-hot encoding
- Need the hashing fn to generate numbers that are as random as possible
- With strings take care of text encoding. Accents, etc, can be visually the same but encoded differently.
    - Likely want to normalise
- Collisions: different inputs -> same hashed output
    - smaller hash size leads to more collisions
- Hashing reduces interpretability of linear models
- Using hash signs cancels out most collisions
- Can use a new hash to generate interaction terms
    - feed hashed value into new hashing fn



## Model Interpretation
- Apply hashing trick to all features
- In GLM then have a coefficient per feature value
    - This gives "average effect" per feature
