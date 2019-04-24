## DFA

**Exercise 1**  
Describe the minimum DFA that recognizes the language of the words over {a,b} which have an even number of a’s.

```
  a b
P I P +
I P I
```

**Exercise 2**  
Describe the minimum DFA that recognizes the language of words over {a,b} with an even number of a’s, and an even number of b’s.

```
  a b
1 4 2 +
2 3 1
3 2 4
4 1 3
```

**Exercise 3**  
Describe the minimum DFA that recognizes the language of words over {a,b} with an odd number of a’s or an odd number of b’s.

```
  a b
1 4 2
2 3 1 +
3 2 4 +
4 1 3 +
```

**Exercise 4**  
Describe the minimum DFA that recognizes the words over {a,b} that end in a.

```
  a b
1 2 1
2 2 1 +
```

**Exercise 5**  
Describe the minimum DFA that recognizes the words over {a,b} ending with bba.

```
  a b
1 1 2
2 1 3
3 4 3
4 1 2 +
```

**Exercise 6**  
Describe the minimum DFA that recognizes the words over {a,b} ending with babab.

```
  a b
1 1 2
2 3 2
3 1 4
4 5 2
5 1 6
6 5 2 +
```

**Exercise 7**  
Describe the minimum DFA that recognizes the words over {a,b} such that the symbol a appears in the third from the last position, and the symbol b appears in the penultimate position.

```
  a b
1 2 1
2 2 3
3 5 4
4 2 1 +
5 2 3 +
```

**Exercise 8**  
Describe the minimum DFA that recognizes the words over {a,b} such that to the left of each occurrence of a there is an even number of b’s.

```
     a    b   
1    1    2    +
2    pozo 1    +
pozo pozo pozo
```

**Exercise 9**  
Describe the minimum DFA that recognizes the words over {a,b} such that to the right of each occurrence of a there is an even number of b’s.

```
     a    b   
1    2    1    +
2    2    3    +
3    pozo 2   
pozo pozo pozo
```

**Exercise 10**  
Describe the minimum DFA that recognizes the language of the words over {a,b} such that every prefix of length greater than or equal to 3 has an even number of a’s or an even number of b’s.

```  
  a b
1 2 3 +
2 4 5 +
3 5 4 +
4 6 7 +
5 7 6 +
6 4 8 +
7 8 4 +
8 8 8
```

**Exercise 11**  
Describe the minimum DFA that recognizes the language of the words over {a,b} such that every prefix of length greater than or equal to 3 has an even number of a’s or an odd number of b’s.

```
  a b
1 2 3 +
2 5 4 +
3 4 5 +
4 3 6 +
5 6 3 +
6 6 6
```

**Exercise 13**  
Describe the minimum DFA that recognizes the language of the words over {a,b} whose subwords of length 3 have an even number of a’s or an even number of b’s.

```
  a b
1 1 1 +
```

**Exercise 14**  
Describe the minimum DFA that recognizes the words over {a,b} such that, if they start with bb, then they do not contain aa.

```
  a b
1 3 2 +
2 3 4 +
3 3 3 +
4 5 4 +
5 6 4 +
6 6 6
```

**Exercise 15**  
Describe the minimum DFA that recognizes the words over {a,b} that do not contain the subword bbb.

```
  a b
1 1 2 +
2 1 3 +
3 1 4 +
4 4 4
```

**Exercise 16**  
Describe the minimum DFA that recognizes the words over {a,b} that do not contain the subword bab.

```
  a b
1 1 2 +
2 3 2 +
3 1 4 +
4 4 4
```

**Exercise 17**  
Describe the minimum DFA that recognizes the words over {a,b} that end in aaa, and do not contain aba or bab.

```
  a b
A B C
B D E
C F C
D G E
E H C
F D H
G G E +
H H H
```

**Exercise 18**  
Describe the minimum DFA that recognizes the words over {a,b,c} that have at most one ocurrence of the subword abc.

```
  a b c
1 2 1 1 +
2 2 3 1 +
3 2 1 4 +
4 5 4 4 +
5 5 6 4 +
6 5 4 7 +
7 7 7 7
```

**Exercise 19**  
Describe the minimum DFA that recognizes the words over {a,b,c} such that between every two occurrences of b there are at least two occurrences of a.

```
  a b c
1 1 2 1 +
2 3 4 2 +
3 1 4 3 +
4 4 4 4
```

**Exercise 20**  
Describe the minimum DFA that recognizes the words over {0,1} such that interpreted in binary represent a natural number multiple of 2 (in particular, the empty word represents 0, which is multiple of 2).  
(Para estos ejercicios de múltiplos en binario, os recomiendo [este video](https://www.youtube.com/watch?v=UWrhRBfF6vM) que explica como hacerlo para cualquier número)

```
  0 1
A A B +
B A B
```

**Exercise 21**  
Describe the minimum DFA that recognizes the words over {0,1} such that interpreted in binary represent a natural number multiple of 3 (in particular, the empty word represents 0, which is multiple of 3).

```
  0 1
A A B +
B C A
C B C
```

**Exercise 22**  
Describe the minimum DFA that recognizes the words over {0,1} such that interpreted in binary represent a natural number which is not multiple of 3 (in particular, the empty word represents 00, which is multiple of 3).

```
  0 1
A A B
B C A +
C B C +
```

**Exercise 23**  
Describe the minimum DFA that recognizes the words over {0,1} such that interpreted in binary represent a natural number multiple of 4 (in particular, the empty word represents 0, which is multiple of 4).

```
  0 1
A A B +
B C B
C A B
```

**Exercise 24**  
Describe the minimum DFA that recognizes the words over {0,1} such that interpreted in binary represent a natural number which is not multiple of 4 (in particular, the empty word represents 0, which is multiple of 4).

```
  0 1
A A B 
B C B +
C A B +
```

**Exercise 25**  
Describe the minimum DFA that recognizes the words over {0,1} such that interpreted in binary represent a natural number multiple of 5 (in particular, the empty word represents 0, which is multiple of 5).

```
  0 1
A A B +
B C D
C E A
D B C
E D E
```

**Exercise 26**  
Describe the minimum DFA that recognizes the words over {a,b} such that every subword with length 3 has exactly two a’s.

```
  a b  
1 2 3 +
2 4 5 +
3 6 7 +
4 8 5 +
5 6 8 +
6 4 8 +
7 8 8 +
8 8 8
```

**Exercise 27**  
Describe the minimum DFA that recognizes the words over {a,b} whose prefixes of odd length have the propierty that their number of b’s equals their number of a’s plus 1.

```
  a b
1 2 3 +
2 2 2
3 1 4 +
4 3 2 +
```

**Exercise 28**  
Describe the minimum DFA that recognizes the words over {a,b} whose suffixes of odd length have the propierty that their number of b’s equals their number of a’s plus 1.

```
  a b   
1 2 3 +
2 4 3  
3 2 6 + 
4 7 5  
5 4 6  
6 5 7 +
7 7 7
```
