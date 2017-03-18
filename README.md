This is a set of quantum circuit macros using TikZ.
The naming convention is attempted as close as the well-established Qcircuit LaTeX package.
With the powerful TikZ support, you may find drawing quantum circuits using this package is as enjoyable as typing equations in LaTeX.

Yet, the reality is that *This is a Work-in-Progress project*.
Currently, the design philosophy is the following:

1. Allow layer-by-layer circuit building.
    In this aspect, one can define a quantum circuit grid by defining a matrix with a particular size. The quantum circuit lines will be drawn automatically as the bottom layer according to the size of the circuit.
    Then, circuit elements can be placed in the matrix as matrix elements on top of the circuit lines.
    By using a background color of the circuit elements the same as the page, the lines going through the circuit elements will be completely covered and seemingly naturally connect with other circuit elements.

2. On top of the circuit/matrix element layer, one should be able to address different positions (with a reference label) and make circuit lines (quantum or classical), branched-out elements and phantom blocks to draw flexible circuit diagram.

At this point, the framework of the first aspect of the design philosophy has been roughly implemented and demonstrated in the Tutorial.tex file, which you can compile and review.
The second aspect of the design philosophy is guaranteed by the nature of the TikZ and matrix drawing packages in LaTeX.
More works may be done especially for the following directions:

1. Implement and demonstrate an easy way to address and draw circuit elements at arbitrary given positions while spacing circuit elements nicely.

2. Define a matrix layer without the bottom quantum circuit line layer to make the circuit drawing more flexible for sparse circuit diagrams and to put elements below the circuit lines easily.

3. More circuit elements need to be defined in a consistent way so that global variables like the background color and scaling factor of circuit elements can be unified in one place.


More thorough thoughts and discussions are welcome!
Coding contributions are appreciated!
