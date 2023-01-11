# linear_regression_nx_axon

Goal: learning a bit of `Nx` and `Axon`, and how to use `Livebook` and `Vegalite` by playing with linear regression.


I take a "straightforward" model made of points in the form `(i, i+:rand.uniform)` in a range `1..50`. 
I want to find the coefficients of the best linear fit to this set.


I start by calculating the exact solution with `Nx` matrices, in other words by playing with tensors, `transpose` and `LinAlg.inverse`.
Then I use statistical formulas to run this calculations.

Then approaching the solution with a gradient descent. This time, I use the `.grad` macro. 
Some graphics are added to understand the importance of coefficients.

Finally, a first encounter with `Axon` by using the most basic Neural Network. The activation is `:linear` and the loss is `: mean_squared_error`. It is important to use `compile: EXLA`.


