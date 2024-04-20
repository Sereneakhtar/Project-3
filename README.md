# Project-3
This project implements a theorem prover using Wang's Algorithm in Prolog. The goal is to prove the validity of logical sequents by applying transformation rules to simplify the sequent until it can be proven or deemed unprovable. 

### Intructions:
1. Project Instructions:
  - Implement a theorem prover using Prolog based on Wang's Algorithm.
  - The theorem prover will handle sequents of the form 'Premises' => 'Conclusion'.
2. Usage:
  - Open the 'thmpv.pl' file in a Prolog interpreter.
  - Consult the file by executing 'consult('thmpv.pl').
  - Use the 'run/2' predicate to start the theorem proving process. Example usage:
    ```prolog
       run([p ^ q], [p]).
    ```
  - This will attempt to prove the sequent 'p ^ q => p'
3. Transformation Rules:
  - Implement transformation rules based on Wang's algorithm to simplify sequents:
      - 'Negation rule' : Handles negation ('~').
      - 'Conjunction rule' : Handles conjunction ('^').
      - 'Disjunction rule' : Handles disjunction ('v').
      - 'Implication rule' : Handles implication ('->').
      - 'Branching rule' : HSplits seuqnets based on certain connectives
4. Testing:
  - Thoroughly test the theorem prover with vairous input sequents tp ensure correctness and completeness.
  - Check both proven and unprovable sequents to validate the implementation
5. Submission:
  - Prepare a submission zip file containing:
      - 'README.md' : Descriptoin of the project, usage instructions, and implementation details.
      - 'thmpv.pl' : Complete prolog code for the theorem prover, incudling all implemented rules.
   
### Notes:
1. Prolog Knowledge:
  - Basic knowledge of Prolog Programming is required to understand and complete the project
2. Project Scope:
  - Focusing on implementing transformation rules accurately and handling various logical connectives.
3. Memory Issues:
  - If encountering memory problems during testing, consier adjusting memory settings or optimizing the code. Example:
    ```prolog
       ?- run([p ^ q], [p]).
       Is p ^ q => p?: We can derive the conclusion from the premises.
       true
