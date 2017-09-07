# Lambda Calculus Bonus Exercises

## Questions

_Borrowed from [CSE340](https://www.youtube.com/watch?v=KoIdCHDbpMI) at Arizona State University and [CMSC 330](http://www.cs.umd.edu/class/spring2011/cmsc330/) at the University of Maryland_

### Parentheses
Use parentheses to make the order of evaluation explicit in the following expressions.

1. `λx. x z λy. x y`

2. `(λx. x z) λy. w λw. w y z x`

3. `λx. x y λx. y x`

### Free variables
Identify all the free variables in the following expressions.

1. `λx. x z λy. x y`

2. `(λx. x z) λy. w λw. w y z x`

3. `λx. x y λx. y x`

### β-reduction
Reduce the following expressions as much as possible.

1. `(λx. x λy. λz. z y x)(y z)`

2. `(λn. λf. λx. f(n f x))(λx. λf. x x x x f)`

3. `(λx. x(λx. λy. y)(λy. λx. y))(λx. λy. y)`

4. `(λx. λy. xy)(λz. (λc. y) z)`

5. `(λx. λy. x y)(λz. (λc. c y) z)`

6. `(λx. x q)(λy. y y y)`

7. `(λc. c(λx. (λx. λy. y))(λx. λy. x))(λq. q)`

8. `(λz. z)(λy. y y)(λx. x a)`

9. `(λz. z)(λz. z z)(λz. z y)`

10. `(λx. λy. x y y)(λa. a) b`

11. `(λx. λy. x y y)(λy. y) y`

12. `(λx. x x)(λy. y x) z`

13. `(λx. (λy. (x y)) y) z`

14. `((λx. x x)(λy. y))(λy. y)`

15. `(((λx. λy. (x y))(λy. y)) w)`

16. `(λx. y)((λy. y y y)(λx. x x x))`
