##Edge cases:
1. Missing 2D map should exit without segfault and without memory leaks when used valgrind
2. 2d map should check for wrong chars/unacceptable chars before memory allocation and exit without segfault and without memory leaks when used valgrind
   - Acceptable chars are 0, 1, W, E, N, S and most importantly, space.
3. 
