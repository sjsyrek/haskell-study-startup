# Lambda Calculus Bonus Exercises

## Answers

_Borrowed from [CSE340](https://www.youtube.com/watch?v=KoIdCHDbpMI) at Arizona State University and [CMSC 330](http://www.cs.umd.edu/class/spring2011/cmsc330/) at the University of Maryland_

### Parentheses

1. `λx. x z λy. x y`  
`(λx. ((x z)(λy. (x y))))`

2. `(λx. x z) λy. w λw. w y z x`  
`((λx. (x z))(λy. (w (λw. (((w y) z) x)))))`

3. `λx. x y λx. y x`  
`(λx. ((x y)(λx. (y x))))`

### Free variables

1. `λx. x z λy. x y`  
`(λx. ((x `_**z**_`) (λy. (x y))))`

2. `(λx. x z) λy. w λw. w y z x`  
`((λx. (x `_**z**_`)) (λy. (`_**w**_` (λw. ((((w y) `_**z**_`) `_**x**_`))))))`

3. `λx. x y λx. y x`  
`(λx. ((x `_**y**_`) (λx. (`_**y**_` x))))`

### β-reduction

1. `(λx. x λy. λz. z y x)(y z)`  
`(λx. x(λy. (λz. z y x)))(y z)`  
`(λx. x(λy1. (λz1. z1 y1 x)))(y z)`  
`y z(λy1. λz1. z1 y1 y z)`  
`y z(λy1. λz1. z1 y1 yz)`  

2. `(λn. λf. λx. f(n f x))(λx. λf. x x x x f)`  
`(λn. λf. λx. f(n f x))(λx. λg. x x x x g)`  
`λf. λx. f((λx. λg. x x x x g)(f x))`  
`λf. λx. f((λg. f f f f g)(x))`  
`λf. λx. f(f f f f x)`  
`λfx. f f f f f x`

3. `(λx. x(λx. λy. y)(λy. λx. y))(λx. λy. y)`  
`(λx. x(λx. λy. y)(λy. λx. y))(λp. λq. q)`  
`(λp. λq. q)(λx. λy. y)(λy. λx. y)`  
`(λq. q)(λy. λx. y)`  
`λy. λx. y`

4. `(λx. λy. xy)(λz. (λc. y) z)`  
`λy. ((λz. (λc. y) z)(y))`  
`λy1. ((λz. (λc. y) z)(y))`  
`λy1. ((λc. y)(y))`  
`λy1. y`

5. `(λx. λy. x y)(λz. (λc. c y) z)`  
`(λy1. (λz. (λc. c y) z)(y1))`  
`(λy1. (λc. c y)(y1))`  
`λy1. y1 y`

6. `(λx. x q)(λy. y y y)`  
`(λy. y y y)(q)`  
`q q q`

7. `(λc. c(λx. (λx. λy. y))(λx. λy. x))(λq. q)`  
`(λq. q)(λx. (λx. λy. y))(λx. λy. x)`  
`(λx. (λx. λy. y))(λx. λy. x)`  
`(λx. λy. y)`  
`λx. λy. y`

8. `(λz. z)(λy. y y)(λx. x a)`  
`(λz. z)(λy. y y)(λx. x a)`  
`(λy. y y)(λx. x a)`  
`(λx. x a)(λx. x a)`  
`(λx. x a) a`  
`a a`

9. `(λz. z)(λz. z z)(λz. z y)`  
`(λz. z)(λz. z z)(λz. z y)`  
`(λz. z z)(λz. z y)`  
`(λz. z y)(λz. z y)`  
`(λz. z y) y`  
`y y`

10. `(λx. λy. x y y)(λa. a) b`  
`(λx. λy. x y y)(λa. a) b`  
`(λy. (λa. a) y y) b`  
`(λa. a) b b`  
`b b`

11. `(λx. λy. x y y)(λy. y) y`  
`(λx. λy. x y y)(λy. y) y`  
`(λx. λa. x a a)(λy. y) y`  
`(λa. (λy. y) a a) y`  
`(λy. y) y y`  
`y y`

12. `(λx. x x)(λy. y x) z`  
`(λx. x x)(λy. y x) z`  
`(λy. y x)(λy. y x) z`  
`(λy. y x) x z`  
`x x z`

13. `(λx. (λy. (x y)) y) z`  
`(λx. (λy. (x y)) y) z`  
`(λx. (λa. (x a)) y) z`  
`(λa. (z a)) y`  
`z y`

14. `((λx. x x)(λy. y))(λy. y)`  
`((λx. x x)(λy. y))(λy. y)`  
`((λy. y)(λy. y))(λy. y)`  
`(λy. y)(λy. y)`  
`λy. y`

15. `(((λx. λy. (x y))(λy. y)) w)`  
`(((λx. λy. (x y))(λy. y)) w)`  
`(((λx. λa. (x a))(λy. y)) w)`  
`((λa. ((λy. y) a)) w)`  
`(λy. y) w`  
`w`

16. `(λx. y)((λy. y y y)(λx. x x x))`  
`y`  
_or_  
`(λx. y)((λx. x x x)(λx. x x x)(λx. x x x))`  
_...ad infinitum_
