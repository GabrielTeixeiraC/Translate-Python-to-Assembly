# Translate Python to Assembly
This is a Computer Organization assignment, in which I translated two procedures in pseudocode into Python and then translated the Python codes into Risc-V Assembly language.

The first procedure receives a starting number (s) and a position number (n) and returns the n-th number of the sequence below starting in s:

    An+1 = An/2 if An is even 
    or
    An+1 = 3 * An + 1 if An is odd
    
The sequence finishes when it gets to 1. If n > number of elements in the sequence, return 0.

The second procedure is:

    rec_selection(vector, num_elem):
      if num_elem is bigger than 2:
        pos = index	of vector's biggest element;
      swap vector[pos] and vector[num_elem - 1];
      rec_selection(vector, num_elem - 1);
      else:
        return
