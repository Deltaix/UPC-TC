## CFG
**Exercise 1**  
Write a non-ambiguous CFG generating the language over {a,b} where the first half of each word only contains a’s and the second half only contains b’s.

```
S -> aSb |
```

**Exercise 2**  
Write a non-ambiguous CFG generating the words over {a,b,c} such that there is an occurrence of cc exactly at the middle, to its left there are only a’s (and there is at least one a), and to its right there are only b’s (and there is at least one b). Note that, since the only occurrence of c must be exactly at the middle, the number of a’s must be equal to the number of b’s.

```
S -> aSb | X
X -> acb
```

**Exercise 3**  
Write a non-ambiguous CFG generating the words of the form a<sup>i</sup>b<sup>j</sup> where the number of a’s is at least the number of b’s.

```
S -> aS | X
X -> aXb |
```

**Exercise 4**  
Write a non-ambiguous CFG generating the words of the form a<sup>i</sup>b<sup>j</sup> where the number of a’s is at most the number of b’s.

```
S -> Sb | X
X -> aXb |
```

**Exercise 5**  
Write a non-ambiguous CFG generating the words of the form a<sup>i</sup>b<sup>j</sup> where the number of b’s is at least twice the number of a’s.

```
S -> Sb | X
X -> aXbb |
```

**Exercise 6**  
Write a CFG generating the words of the form a<sup>i</sup>b<sup>j</sup> where the number of b’s is at most twice the number of a’s.

```
S -> aSbb | aSb | aS | 
```

**Exercise 7**  
Write a non-ambiguous CFG generating the words of the form a<sup>i</sup>b<sup>j</sup> where the number of b’s is at most twice the number of a’s.

```
S -> aXb | aSbb | aX |
X -> aX |
```

**Exercise 8**  
Write a non-ambiguous CFG generating the words of the form a<sup>i</sup>b<sup>j</sup> where the number of a’s is at least the number of b’s, but at most twice the number of bb’s.

```
S -> aaSb | X
X -> aXb |
```

**Exercise 9**  
Write a non-ambiguous CFG generating the words of the form a<sup>i</sup>b<sup>j</sup> where the number of a’s is at least the number of b’s, or it is at most twice the number of bb’s.

```
S -> AB
A -> aA |
B -> bB |
```

**Exercise 10**  
Write a non-ambiguous CFG generating the words of the form a<sup>i</sup>b<sup>j</sup>c<sup>k</sup> such that the number of a’s coincides with the number of b’s plus the number of c’s.

```
S -> aSc | X
X -> aXb |
```

**Exercise 11**  
Write a non-ambiguous CFG generating the words of the form a<sup>i</sup>b<sup>j</sup>c<sup>k</sup> such that the number of b’s coincides with the number of a’s plus the number of c’s.

```
S -> XY
X -> aXb |
Y -> bYc |
```

**Exercise 12**  
Write a CFG (which will be ambiguous) generating the words of the form a<sup>i</sup>b<sup>j</sup>c<sup>k</sup> where the number of a’s equals the number of b’s, or the number of b’s equals the number of c’s, or the number of c’s equals the number of a’s.

```
S -> XC | AY | Z
X -> aXb |
C -> Cc |
A -> aA |
Y -> bYc |
Z -> aZc | B
B -> bB |
```

**Exercise 16**  
Write a non-ambiguous CFG generating the palindromic words over {a,b}.

```
S -> aSa | bSb | a | b | 
```

**Exercise 18**  
Write a non-ambiguous CFG generating the palindromic words over {a,b} with some occurrence of a and some occurrence of b.

```
S -> aXa | bYb
X -> aXa | bZb | b
Y -> bYb | aZa | a
Z -> aZa | bZb | a | b |
```

**Exercise 20**  
Write a CFG generating the language of the well-parenthesized words over {(,)}. For example, ()(())()(()) and (((()())))(((()()))) are well-parenthesized words, whereas )()( and (()(() are not. One way to define more precisely this language is to describe it as the set of words that can be reduced to the empty word by successive applications of the rewrite rule ()→λ.

```
S -> (S)S |
```
