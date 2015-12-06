# mathematica-cheat-sheet
How to do some simple, but non-obvious stuff in Mathematica

Matrices
--------

#### Build from folding a list

```mathematica
(* ArrayReshape[list, {n, n}] *)

In[1]:= ArrayReshape[Alphabet[], {3, 3}]
Out[1]= {{"a", "b", "c"}, {"d", "e", "f"}, {"g", "h", "i"}}
```
