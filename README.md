# Implementation of SLR parser
### Form of grammar
- Put each rule in a single line
- Rules must be in form LHS => RHS
- NON-TERMINALS
    - must start with (`)
    - be UPPERCASE
    - use only [A-Z] and (_) for NONTERMINALS
- Terminals must be lower case
- If there are many rhs of a lhs
    - put all in the same line
    - separate them with (|)
    - i.e: X => Y | Z | !εpslon
- Use the form (!εpslon) for writing epslons
- Example grammar:
    - \`E => \`T \`E_
    - \`E_ => + \`T \`E_ | !εpslon
    - \`T => \`F \`T_
    - \`T_ => * \`F \`T_ | !εpslon
    - \`F => ( \`E ) | id
### Requirements
- python 3
- numpy
- Pandas
- Matplotlib
- Networkx
- pygraphviz (optional)
