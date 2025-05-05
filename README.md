# programming-paradigms-homework-1-solved
**TO GET THIS SOLUTION VISIT:** [Programming Paradigms Homework 1 Solved](https://www.ankitcodinghub.com/product/programming-paradigms-homework-1-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;100194&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;Programming Paradigms Homework 1 Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
1 Symbolic differentiation 1.1 Polynomial expressions

In this assignment you will need to implement the tools for symbolic differentiation of expressions. Symbolic differentiation computes derivative of a given expression symbolically (i.e. as an expression), for example, given (1 + 2x)(x + y) the computed partial derivative with respect to variable y is 1 + 2x.

For start we will consider only expressions involving numeric constants, variables, binary addition and multiplication. The expressions will be given as valid Racket terms, for example:

</div>
</div>
<div class="layoutArea">
<div class="column">
‘(+ 1 x)

‘(* 2 y) ‘(*(+1(*2x))(+xy))

</div>
<div class="column">
; 1 + x

; 2y

; (1+2x)(x+y)

</div>
</div>
<div class="layoutArea">
<div class="column">
To work with these expressions, you need to be able to traverse its structure. You can use number? predicate to check whether an expression is a number.

Exercise 1.1 (⋆). Implement the following predicates and functions:

</div>
</div>
<div class="layoutArea">
<div class="column">
(define (variable? expr) …)

(define (sum? expr) …)

(define (summand-1 expr) …)

(define (summand-2 expr) …)

(define (product? expr) …)

(define (multiplier-1 expr) …) ; extract first multiplier from a product (define (multiplier-2 expr) …) ; extract second multipler from a product

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>; check whether a given expression is a variable
; check whether a given expression is a sum
; extract first summand from a sum
; extract second summand from a sum
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>; check whether a given expression is a product
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
Now, whenever we have an expression we can check what kind of expression we have and decompose it into its constituent subexpressions.

Exercise 1.2 (⋆). Implement a recursive function derivative that computes a symbolic derivative of a given expression with respect to a given variable. At this point you are not expected to simplify expressions after differentiation:

(derivative ‘(+ 1 x) ‘x) ; ‘(+ 0 1)

(derivative ‘(* 2 y) ‘y) ; ‘(+ (* 0 y) (* 2 1))

(derivative ‘(* (+ x y) (+ x (+ x x))) ‘x)

; ‘(+ (* (+ 1 0) (+ x (+ x x))) (* (+ x y) (+ 1 (+ 1 1))))

Exercise 1.3 (⋆⋆). Implement a recursive function simplify that simplifies an expression using the following rules:

1. 0+e=eforallexpressionse,

2. e+0=eforallexpressionse,

3. 1∗e=eforallexpressionse,

4. e∗1=eforallexpressionse,

5. 0∗e=0forallexpressionse,

6. e∗0=0forallexpressionse,

7. sums and products of numeric constants should be computed.

Examples:

(simplify ‘(+ 0 1)) ;1

(simplify ‘(+ (* 0 y) (* 2 1))) ;2

(simplify ‘(+ (* (+ 1 0) (+ x (+ x x))) (* (+ x y) (+ 1 (+ 1 1))))) ; ‘(+ (+ x (+ x x)) (* (+ x y) 3))

Hint: it might be easier to implement a non-recursive function simplify-at-root that only simplifies expression if it matches exactly left-hand side of one of the rules. Then use simplify-at-root to implement a recursive function simplify.

Exercise 1.4 (⋆ ⋆ ⋆). Implement function normalize that simplifies any expression down to a poly- nomial of its variables. To achieve that you need to open parentheses using distributive property of multiplication over addition: x(y + z) = xy + xz. You will also need to simplify similar terms: xy + 2yz + 3xy = 4xy + 2yz.

Exercise 1.5 (⋆). Implement a recursive function to-infix that converts an expression into an infix form:

(to-infix ‘(+ (+ x (+ x x)) (* (+ x y) 3)) ; ‘((x + (x + x)) + ((x + y) * 3)

</div>
</div>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
1.2 More functions

Exercise 1.6 (⋆). Update functions derivative and simplify to support the following functions (here e, e1 and e2 denote arbitary expressions):

1. exponentiation: ee2 1

2. trigonometric functions: sin e, cos e, tan e

3. natural logarithm: log e

Exercise 1.7 (⋆⋆). Update functions derivative and simplify to support the following polyvariadic1

sums and products:

(derivative ‘(+ 1 x y (* x y z)) ‘x)

; ‘(+ 0 1 0 (+ (* 1 y z) (* x 0 z) (* x y 0)))

(simplify ‘(+ 0 1 0 (+ (* 1 y z) (* x 0 z) (* x y 0)))) ; ‘(+ 1 (* y z))

1.3 Gradient

Exercise 1.8 (⋆⋆). Implement a function variables-of that returns a (sorted) list of distinct variables used in a given expression:

(variables-of ‘(+ 1 x y (* x y z))) ; ‘(x y z)

Exercise 1.9 (⋆⋆). Implement a function gradient that returns a gradient of a multivariable expres- sion (given explicitly the list of variables). Recall that the gradient ∇f is a vector consisting of partial

</div>
</div>
<div class="layoutArea">
<div class="column">
derivatives:

</div>
<div class="column">
􏰁∂e ∂e ∂e􏰂⊤ ∇e= ∂x ∂x ···∂x

</div>
</div>
<div class="layoutArea">
<div class="column">
12n Represent gradient in Racket as a list of expressions:

</div>
</div>
<div class="layoutArea">
<div class="column">
(gradient ‘(+ 1 x y (* x y z)) ‘(x y z)) ; ‘((+ 1 (* y z)) (+ 1 (* x z)) (* x y))

</div>
</div>
<div class="layoutArea">
<div class="column">
1“polyvariadic” means that a function or operator can support arbitrary number of arguments; for example, + in Racket can accept as many arguments, as user wants: (+ 1 2 3 4) computes to 1+2+3+4 = 10.

</div>
</div>
<div class="layoutArea">
<div class="column">
3

</div>
</div>
</div>
