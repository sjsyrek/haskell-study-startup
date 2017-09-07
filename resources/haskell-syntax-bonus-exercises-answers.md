# Haskell Syntax Bonus Exercises

## Answers

### Expression forms

1. normal form
2. normal form
3. weak head normal form
4. redex
5. redex (but reduces to weak head normal form)
6. redex
7. weak head normal form
8. weak head normal form
9. normal form
10. redex
11. weak head normal form
12. weak head normal form
13. normal form
14. weak head normal form
15. weak head normal form
16. normal form
17. weak head normal form
18. weak head normal form
19. redex
20. weak head normal form
21. redex
22. weak head normal form
23. weak head normal form
24. weak head normal form
25. normal form

### Application operator

1. `take 1 $ drop 1 [1..10]`
2. `fst $ swap $ swap $ (2,3)`
3. `unwords $ words $ str ++ "!"`
4. `intersect [2,4,6,8] $ nub $ union [1,2,2,3,4,5,5,5,6,6,7] [2,4,6,8]`
5. `map snd $ zip (zipWith ($) [(+3),(+2),(+1)] [1,2,3]) "abc"`

### let vs. where

1. `whiteLines colors = intersperse w colors
      where w = "white"`
2. `abs n = if n < 0 then n' else n
      where n' = negate n`
3. `f x y z = a <= 0
      where a = x * (y - z)`
