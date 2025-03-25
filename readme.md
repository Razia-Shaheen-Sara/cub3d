***Edge cases***

**Input check**

1. no file
2. wrong file
3. multiple files
   **In file**

1. Empty file
2. File with only whitespaces
3. 2d map in the beginning
4. Missing 2d map
5. missing color
6. missing texture
7. color and texture lines in between each other


**Texture line**

1. texture path not ending with png
2. spaces/tabs after png shuld be valid
3. NO spaces between identifier and texture path (should be invalid)
4. wrong name of texture path


**Color Line**

1. multiple delimeter within color line colors should be invalid
2. spaces and tabs after color line valid


**2d map**

1. **Missing 2D map** should exit without segfault and without memory leaks when used valgrind
2. 2d map should check for **wrong chars/unacceptable chars in 2d map** before memory allocation and exit without segfault and without memory leaks when used valgrind
   - Acceptable chars are 0, 1, W, E, N, S and most importantly, space.
3. space in non playable area-- should be valid
4. 2 players
5. Player not enclosed

