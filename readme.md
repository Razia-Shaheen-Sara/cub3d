***Edge cases***
**Run **ALL** invalid cases and one valid case with valgrind**


**Input check**

1. no file
2. wrong file
3. multiple files
4. Space after files


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
2. spaces/tabs after png should be valid
3. NO spaces between identifier and texture path (should be invalid)
4. wrong name of texture path(should be invalid with no segfault exit)
5. Double texture files for same direction - invalid


**Color Line**

1. multiple delimeter within color line colors should be invalid
2. spaces and tabs after color line valid
3. Spaces and tabs in between color numbers should be valid
4. All 255 or all 0 should make black / white
5. No spaces and tabs between identifier and numbers should be invalid
6. Double color line for same area - invalid


**2d map**

1. **Missing 2D map** should exit without segfault and without memory leaks when used valgrind
2. 2d map should check for **wrong chars/unacceptable chars in 2d map** before memory allocation
   - Acceptable chars are 0, 1, W, E, N, S and most importantly, "space outside wall".
3. space in non playable area-- should be valid
4. 2 players invalid
5. Player not enclosed is invalid\n


For all cases, should not leak from get_next_line (not a major issue but shows in valgrind as 2 bytes still reachable) 
