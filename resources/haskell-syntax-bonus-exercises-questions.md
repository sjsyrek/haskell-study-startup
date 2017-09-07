# Haskell Syntax Bonus Exercises

## Questions

### Expression forms
Identify the form (_normal form_, _weak head normal form_, or _redex_) of each of the following expressions:

1. `23`
2. `(2,3)`
3. `\x -> 2 + 3`
4. `(\x -> x + 2) 3`
5. `(\x -> \y -> x + y) 2`
6. `2 + 3`
7. `(2 + 2, 3 + 3)`
8. `Just (2 + 3)`
9. `Just 5`
10. `[1,2,3] ++ [4,5,6]`
11. `Just $ [1,2,3] ++ [4,5,6]`
12. `[Just 1, Just 2, Just (2 + 3)]`
13. `[Just (1,2), Just (2,3), Just (4,5)]`
14. `\x -> \y -> \z -> x + y(z)`
15. `\x -> ((\y -> y + 1) 1) + x`
16. `[[1,2,3]]`
17. `[1,2,3] : []`
18. `[1 + 1]`
19. `[1] ++ []`
20. `(+) 1`
21. `(+) 1 2`
22. `print`
23. `div (1 + 2 * 3 - 4)`
24. `(+ 2)`
25. `(- 3)`

### Application operator
Replace the parentheses with the `$` operator in the following expressions:

1. `take 1 (drop 1 [1..10])`
2. `fst (swap (swap (2,3)))`
3. `unwords (words (str ++ "!"))`
4. `intersect (nub (union [1,2,2,3,4,5,5,5,6,6,7] [2,4,6,8])) [2,4,6,8]`
5. `map snd (zip (zipWith ($) [(+3),(+2),(+1)] [1,2,3]) "abc")`

### let vs. where
Rewrite the following `let` expressions to use `where` instead.

1. `whiteLines colors = let w = "white"
      in intersperse w colors`
2. `abs n = let n' = negate n
      in if n < 0 then n' else n`
3. `f x y z = let a = x * (y - z)
      in a <= 0`
