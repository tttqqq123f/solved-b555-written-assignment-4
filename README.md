Download Link: https://assignmentchef.com/product/solved-b555-written-assignment-4
<br>
<ol>

 <li>In this question we consider the hard margin SVM formulation as developed in class and thetextbook. Recall that we stated that for this type of optimization problem there is no duality gap. That is, the primal and dual objective functions have the same value at their optimal solutions. Use this fact and other facts developed in class to show that the maximum margin <em>γ</em>∗ can be calculated from the dual solution <em>α</em><sup>∗</sup>. More specifically show that .</li>

 <li>The soft margin SVM formulation developed in class called for minimizing subject to constraints (for all <em>i</em>) 1 − <em>ξ<sub>i </sub></em>− <em>t<sub>i</sub></em>(<em>v<sup>T</sup>φ</em>(<em>x<sub>i</sub></em>) + <em>v</em><sub>0</sub>) ≤ 0 and <em>ξ<sub>i </sub></em>≥ 0.</li>

</ol>

Consider the alternative formulation QSVM that uses a quadratic penalty on <em>ξ<sub>i </sub></em>which is: minimize  subject to constraints (for all <em>i</em>) 1 − <em>ξ<sub>i </sub></em>− <em>t<sub>i</sub></em>(<em>v<sup>T</sup>φ</em>(<em>x<sub>i</sub></em>) + <em>v</em><sub>0</sub>) ≤ 0.

Note that we do not need the constraint <em>ξ<sub>i </sub></em>≥ 0 in this formulation because <em>ξ<sub>i </sub>&lt; </em>0 increases the objective function and makes the constraints harder to satisfy. Develop the dual formulation of QSVM: that is (1) compute the dual objective function, (2) state the dual optimization problem, and (3) argue that QSVM is also a kernel method.

<ol start="3">

 <li>In this problem we show that many machine learning problems have solutions that can beexpressed through kernels. Consider the standard formulation where <em>a<sub>i </sub></em>= <em>w<sup>T</sup>φ</em>(<em>x<sub>i</sub></em>), and where we have a loss function <em>`</em>(<em>a<sub>i</sub>,t<sub>i</sub></em>). For example we might use the square loss <em>`</em>(<em>a<sub>i</sub>,t<sub>i</sub></em>) = (<em>t<sub>i</sub></em>−<em>a<sub>i</sub></em>)<sup>2 </sup>or the classification log loss <em>`</em>(<em>a<sub>i</sub>,t<sub>i</sub></em>) = <em>t<sub>i </sub></em>ln<em>y<sub>i </sub></em>+(1−<em>t<sub>i</sub></em>)ln(1−<em>y<sub>i</sub></em>) where <em>y<sub>i </sub></em>= <em>σ</em>(<em>a<sub>i</sub></em>) etc. But for this question we consider any loss function. In addition consider any regularization function <em>R</em>(<em>b</em>) which is monotonically increasing, where <em>b </em>is a scalar.</li>

</ol>

Now consider a machine learning objective of the form <sup>P</sup><em><sub>i </sub>`</em>(<em>a<sub>i</sub>,t<sub>i</sub></em>) + <em>R</em>(<em>w<sup>T</sup>w</em>).

Show the the optimal solution can be expressed as <em>w </em>= <sup>P</sup><em><sub>i </sub>α<sub>i</sub>φ</em>(<em>x<sub>i</sub></em>) that is, it is a weighted sum of training examples. Note that this shows that predictions on test example <em>z </em>can be computed as <em>w<sup>T</sup>φ</em>(<em>z</em>) = <sup>P</sup><em><sub>i </sub>α<sub>i</sub>K</em>(<em>x<sub>i</sub>,z</em>).

<ol start="4">

 <li>In lecture we provided a general form for optimizing the hyper-parameters of Gaussian ProcessRegression (GPR). In general there is no closed form and we must use some iterative gradient based optimization. Consider GPR where one hyperparameter, <em>θ</em><sub>0</sub>, gives the overall scale of the covariance. Specifically, assume the covariance matrix has the form <em>C</em>(<em>x<sub>n</sub>,</em><em>x<sub>m</sub></em>) = <em>θ</em><sub>0</sub><em>k</em>(<em>x<sub>n</sub>,</em><em>x<sub>m</sub></em>) where <em>k</em>(·<em>,</em>) is any valid kernel. Show that the marginal likelihood can be optimized w.r.t. <em>θ</em><sub>0 </sub>in closed form and develop the solution for <em>θ</em><sub>0</sub>.</li>

</ol>

1