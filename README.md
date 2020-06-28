# create-LR-parser

## Features
- Construct the parsing table
- Trace the parse stack of input string
- Draw the DFA

## Form of grammar
- Put each rule in a single line
- Rules must be in form `LHS => RHS`
- NON-TERMINALS
    - must start with (\`)
    - be UPPERCASE
    - use only `[A-Z]` and (`_`) for NONTERMINALS
- Terminals must be lower case
- If there are many rhs of a lhs
    - put all in the same line
    - separate them with (|)
    - e.g.: `X => Y | Z | !εpslon`
- Use the form (`!εpslon`) for writing epslons
- Example grammar:
    - \`E => \`T \`E_
    - \`E_ => + \`T \`E_ | !εpslon
    - \`T => \`F \`T_
    - \`T_ => * \`F \`T_ | !εpslon
    - \`F => ( \`E ) | id

## Requirements
- python 3
- numpy
- Pandas
- Matplotlib
- Networkx
- pygraphviz (optional)

## Results

![result of SLR parser](https://lh3.googleusercontent.com/wPjIppmlmsLfOCa1wHPafi2hwj4EPPbnj5ZP-SiTYAgurYpSzep35V4-qhnCe1b0JAJPIbSKZfk0e85uitou7qFeGfW9AgjghXDiJf5y_wRcx18LHxKo5p8z1NJATooqkQspPXmL=w1066-h389-no)
