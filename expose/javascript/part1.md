1. Line 9 prints values added: 20
2. Line 13 print final result: 20
3. Since var is function scoped, we could see unexpected behavior outside of the function. Furthermore, since var allows redecarling the same variable it can cause confusion and reduce readability. 
4. Line 9 prints values added: 20
5. Line 13 will print an error because let is block scoped, meaning that outside of the block, result is not accessible.
6. Line 9 prints 0
7. line 13 will print an error because const is the same scope as let, so result is similarily not accessible.