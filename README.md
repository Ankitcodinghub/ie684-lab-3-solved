# ie684-lab-3-solved
**TO GET THIS SOLUTION VISIT:** [IE684 Lab 3 Solved](https://www.ankitcodinghub.com/product/ie684-lab-3-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;97632&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;IE684 Lab 3 Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
Exercise 1: Gradient Descent with Scaling

Recall that in the last lab, when we tried to solve certain problems of the form minx∈Rn f(x) using gradient descent algorithm, we noticed that the algorithm needed a large number of iterations to find the minimizer. As a workaround to avoid such situations, we consider the modified gradient descent scheme illustrated in Algorithm 1.

Input: Starting point x0, Stopping tolerance τ Initialize k = 0

pk = −∇f(xk).

while ∥pk∥2 &gt; τ do

Choose a suitable scaling matrix Dk.

ηk = arg minη≥0 f(xk + ηDkpk) = arg minη≥0 f(xk − ηDk∇f(xk)) xk+1 = xk + ηkDkpk = xk − ηkDk∇f(xk)

k=k+1

end

Output: xk .

Algorithm 1: Gradient Descent Procedure with Scaling

<ol>
<li>Note that in the notebook file shared with you, we provide the motivation for the modified gradient descent
procedure with scaling.
</li>
<li>[R] Consider the function f(x) = 1500×21 + 4x1x2 + x2. Write code to find the Hessian matrix of f and its condition number.</li>
<li>Note that the update step in the modified gradient descent scheme uses a scaled gradient. Thus it becomes important to set up some criteria for choosing the Dk matrix in every iteration. In this exercise, we will assume Dk to be a diagonal matrix. The following questions will help in designing a suitable Dk.</li>
<li>[R] Based on our discussion on condition number and the derivation of the gradient descent scheme with scaling, can you identify and write down the matrix Q whose condition number needs to be analyzed in the new gradient scheme with scaling?</li>
<li>[R] Based on the matrix Q, can you come up with a useful choice for Dk (assuming Dk to be diagonal)?</li>
<li>Write all related code to implement Algorithm 1 to find the minimizer of the function f(x) = 1500×21+4x1x2+x2.</li>
<li>[R] Note down the minimizer and minimum function value of f(x) = 1500×21 + 4x1x2 + x2.</li>
<li>[R] With starting point x0 = (1, 4000) and a stopping tolerance τ = 10−12, find the number of iterations taken by the gradient descent algorithm (without scaling) with exact line search, gradient descent algorithm (without scaling) with backtracking line search, gradient descent algorithm (with scaling) with backtracking line search. For backtracking line search, use α0 = 1, ρ = 0.5, γ = 0.5. Note the minimizer and minimum objective function value in each case. Comment on your observations.</li>
<li>[R] With starting point x0 = (1, 4000) and τ = 10−12, we will now study the behavior of gradient descent algo- rithm (without scaling) with backtracking line search, gradient descent algorithm (with scaling) with backtrack- ing line search, for different choices of α0 . Take γ = ρ = 0.5. Try α0 ∈ {1, 0.9, 0.75, 0.6, 0.5, 0.4, 0.25, 0.1, 0.01}. For each α0, record the final minimizer, final objective function value and number of iterations to terminate, for the gradient descent algorithm (without scaling) with backtracking line search and the gradient descent algorithm (with scaling) with backtracking line search. Prepare a plot where the number of iterations for both the algorithms are plotted against α0 values. Use different colors and a legend to distinguish the plots corresponding to the different algorithms. Comment on the observations. Comment about the minimizers and objective function values obtained for different choices of the α0 values for the two algorithms.</li>
</ol>
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
IE684, IEOR Lab

Lab 03 19-January-2022

10. [R] With starting point x0 = (1, 4000) and τ = 10−12, we will now study the behavior of gradient descent algo- rithm (without scaling) with backtracking line search, gradient descent algorithm (with scaling) with backtrack- ing line search, for different choices of ρ. Take α = 1, γ = 0.5. Try ρ ∈ {0.9, 0.8, 0.75, 0.6, 0.5, 0.4, 0.25, 0.1, 0.01}. For each ρ, record the final minimizer, final objective function value and number of iterations to terminate, for the gradient descent algorithm (without scaling) with backtracking line search and the gradient descent algorithm (with scaling) with backtracking line search. Prepare a plot where the number of iterations for both the algorithms are plotted against ρ values. Use different colors and a legend to distinguish the plots corresponding to the different algorithms. Comment on the observations. Comment about the minimizers and objective function values obtained for different choices of the ρ values for both the algorithms.

</div>
</div>
<div class="layoutArea">
<div class="column">
3

</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
IE684, IEOR Lab Lab 03

Exercise 2:

Consider the function

</div>
<div class="column">
19-January-2022

</div>
</div>
<div class="layoutArea">
<div class="column">
q(x) = 512(x2 − x21)2 + (4 − x1)2.

</div>
</div>
<div class="layoutArea">
<div class="column">
1. [R] Can you design a suitable diagonal matrix Dk for gradient descent algorithm with scaling to solve minx q(x). If you can come up with a suitable choice of Dk, use it in the implementation of Algorithm 1 (with backtracking line search) to find the minimizer of q(x) with starting point x0 = (8,8) and τ = 10−5. Consider α0 = 1,ρ = 0.5, γ = 0.5 for backtracking line search. Comment on your observations when compared to the gradient descent (without scaling) with backtracking line search. If you cannot find a suitable choice of Dk, explain clearly the reasons.

2. If we allow the scaling matrix Dk to be non-diagonal, then a natural choice turns out to be Dk = (∇2f(xk))−1. This choice of Dk yields the popular Newton’s method. Implement Algorithm 1 with this choice of Dk = (∇2f(xk))−1.

3. [R] Based on our discussion on condition number and the derivation of the gradient descent scheme with scaling, can you identify and write down the matrix Q whose condition number needs to be analyzed in the new gradient descent scheme with scaling with Dk = (∇2f(xk))−1?

4. [R] With starting point x0 = (8,8) and a stopping tolerance τ = 10−5, find the number of iterations taken by the gradient descent algorithm (without scaling) with backtracking line search, gradient descent algorithm (with scaling) with backtracking line search. For backtracking line search, use α0 = 1,ρ = 0.5,γ = 0.5. Note the minimizer and minimum objective function value in each case. Comment on your observations. Also note the condition number of the Hessian matrix involved in the gradient descent algorithm (without scaling) with backtracking line search and condition number of the matrix Q involved in the gradient descent algorithm (with scaling) with backtracking line search in each iteration. Prepare a plot depicting the behavior of condition numbers in both algorithms against iterations. Use different colors and legend to distinguish the methods. Comment on your observations.

</div>
</div>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</div>
