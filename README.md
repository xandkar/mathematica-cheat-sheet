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

#### Non-destructive column/row replace

```mathematica
(* ReplacePart[list, rule] *)

In[1]:= ReplacePart[
 {{"a", "b", "c"}, {"d", "e", "f"}, {"g", "h", "i"}},
 {_, 1} -> 0
 ]
Out[1]= {{0, "b", "c"}, {0, "e", "f"}, {0, "h", "i"}}
```
