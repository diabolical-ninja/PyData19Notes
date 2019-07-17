# On the Path to Causal Inference

https://pydata.org/london2019/schedule/presentation/16/


Causal Diagrams Photo
- Y = thing we want to measure
- M = our input to generate effect

A
- Also known as bayesian graph
- Should be DAG

- Backdoor path
    - Ways to get from M -> Y
    - Ignores directionality, thus M -> S -> G -> Y
    - Needs to be controlled for



Collider = Path from A -> C goes via B but A -> B AND C -> B


