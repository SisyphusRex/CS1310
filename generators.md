# Generating Function
represent a sequence of numbers as an algebraic function in which each term in the sequence is a coefficient
of an $`x^{j}`$ term in the function

Example:
* the sequence
  * $`f_{0},f_{1},f_{2},...`$
* is represented by the generating function
  * $`F(x) = f_{0} + f_{1}x + f_{2}x^2 + f_{3}x^3 + ...`$
* $`f_{j}`$ is the coefficient of the $`x^j`$ term

### Geometric Sum
* Each term is x times the previous term
* $`H(x) = \sum_{j=0}^{\infty }x^{j}=\frac{1}{1-x}`$
* sequence is 1,1,1,1...

### Select Oranges in Pack
Three oranges are wrapped in a single pack:
0(x) = 1 + x^3

### Select Apples and Bananas
Create a generating function that describes how many ways to select subsets from a finite set
* One apple and one banana in set
    * 1 + 2x + x^2
    * only two objects are available to select, so no set of size three or more can be selected and coeffecitents of x^(n>2) are zero
    * only 1 way to select 0 objects, 2 ways to select one, and 1 way to select 2
* Two apples and two Bananas in set
    * 1 + 2x + 3x^2 + 2x^3 + x^4
    * a 2-subset can be selected in three ways, so coefficient of x^2 is 3
    * a 3-subset can be selected in two ways
    * a 4-subset can only be selected in one way
* Three apples and one banana in set
    * 1 + 2x + 2x^2 + 2x^3 + x^4

### Short form Long Form
Infinite Supply of one kind of item
    Long: 1 + x + x^2 + x^3 ...
    Short: 1/(1-x)

Selecting from a set of n identical items
    Long: 1 + x + x^2 + ... + x^n
    Short: (1-x^(n+1))/(1-x)

Infinite Supply of identical items grouped in batches of k:
    Long: 1 + x^k + x^(2k) + x^(3k)...
    Short: 1/(1-x^k)

Infinite Supply of two different kinds of items:
    Long: 1 + 2x + 3x^2 + 4x^3 ...
    Short: 1/((1-x)(1-x))= 1/(1-x)^2

One Pack of k size
    1 + x^k

### Product of Generating Functions
the two sets of objects must be distinct (like apples and bananas)
Using the apples and bananas example, pool three apples and two bananas into a set of 5 pieces of fruit
Get generating function for three apples and two bananas
Multiply the generating functions
get coefficient of term fx for selecting x pieces of fruit

### Binomial Theorem
$`(1+x)^{n} = \sum_{j=0}^{n}\binom{n}{j}x^{j}`$