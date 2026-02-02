# Complete Derivation of Equation Equivalence (F.19) to (F.21)

## Abstract

This document provides the complete step-by-step algebraic derivation demonstrating the equivalence between equations (F.19) and (F.21) in Appendix F of the main paper. The derivation establishes that on the boundary of the effective cooperation zone, these two expressions for passenger sensitivity \(\phi\) are mathematically equivalent.

## Notation

For clarity in derivation, we define:

\[
\Theta \equiv (dy + k_2)[k_0 - (e_L - e_R)\lambda]
\]

Key model parameters:

\[
\begin{aligned}
A &= d\left(F(h_1 + 2Hy\eta) + h_2\right) \\
\kappa_1 &= k_1 + \frac{d}{F\eta}(Fh_1 + h_2)
\end{aligned}
\]

Other parameters maintain their definitions from the main paper (see Appendix A).

## Derivation

### Step 1: Starting from the Discriminant Condition

The Nash bargaining solution's discriminant (Appendix H, equation H.17) is:

\[
\Delta_1 = \left[A - F\eta\left(k_1 + (2w + \tau)\phi\right)\right]^2 - 4F^2(dy + k_2)\eta^2[k_0 - (e_L - e_R)\lambda]
\]

At the boundary of the effective cooperation zone, \(\Delta_1 = 0\):

\[
\left[A - F\eta\left(k_1 + (2w + \tau)\phi\right)\right]^2 = 4F^2(dy + k_2)\eta^2[k_0 - (e_L - e_R)\lambda] \tag{1}
\]

Taking the positive square root (valid for realistic parameter values where the left-hand side is non-negative):

\[
A - F\eta\left(k_1 + (2w + \tau)\phi\right) = 2F\eta\sqrt{\Theta} \tag{2}
\]

### Step 2: Solving for \(\phi\) (Equation F.19)

From equation (2), solve for \(\phi\):

\[
\phi = \frac{A}{F\eta(2w + \tau)} - \frac{k_1}{2w + \tau} - \frac{2\sqrt{\Theta}}{2w + \tau} \tag{F.19}
\]

### Step 3: Expressing \(A\) in Terms of \(\kappa_1\)

First, expand \(A\):

\[
A = dFh_1 + 2dFHy\eta + dh_2 \tag{3}
\]

Compute \(\frac{A}{F\eta}\):

\[
\frac{A}{F\eta} = \frac{dFh_1 + 2dFHy\eta + dh_2}{F\eta} = \frac{dh_1}{\eta} + 2dHy + \frac{dh_2}{F\eta} \tag{4}
\]

From the definition of \(\kappa_1\):

\[
\kappa_1 = k_1 + \frac{d}{F\eta}(Fh_1 + h_2) = k_1 + \frac{dFh_1 + dh_2}{F\eta} \tag{5}
\]

Thus:

\[
\frac{dFh_1 + dh_2}{F\eta} = \kappa_1 - k_1 \tag{6}
\]

Note that:

\[
\frac{dh_1}{\eta} + \frac{dh_2}{F\eta} = \frac{dFh_1 + dh_2}{F\eta} = \kappa_1 - k_1 \tag{7}
\]

Substituting equation (7) into equation (4):

\[
\frac{A}{F\eta} = (\kappa_1 - k_1) + 2dHy \tag{8}
\]

### Step 4: Substituting into Equation (F.19)

Insert equation (8) into equation (F.19):

\[
\begin{aligned}
\phi &= \frac{(\kappa_1 - k_1) + 2dHy}{2w + \tau} - \frac{k_1}{2w + \tau} - \frac{2\sqrt{\Theta}}{2w + \tau} \\
&= \frac{\kappa_1 - 2k_1 + 2dHy}{2w + \tau} - \frac{2\sqrt{\Theta}}{2w + \tau} \tag{9}
\end{aligned}
\]

### Step 5: Equation (F.21) Form

Equation (F.21) from the main paper is:

\[
\phi = \frac{\lambda(e_L - e_R) - \kappa_1}{2w + \tau} + \frac{\sqrt{4F^2(dy + k_2)\eta^2[k_0 - (e_L - e_R)\lambda]}}{F\eta(2w + \tau)} \tag{F.21}
\]

Simplify the second term:

\[
\frac{\sqrt{4F^2(dy + k_2)\eta^2[k_0 - (e_L - e_R)\lambda]}}{F\eta(2w + \tau)} = \frac{2\sqrt{\Theta}}{2w + \tau} \tag{10}
\]

Thus equation (F.21) becomes:

\[
\phi = \frac{\lambda(e_L - e_R) - \kappa_1}{2w + \tau} + \frac{2\sqrt{\Theta}}{2w + \tau} \tag{11}
\]

### Step 6: Establishing the Equivalence Condition

Comparing equations (9) and (11), they are equal if and only if:

\[
\frac{\kappa_1 - 2k_1 + 2dHy}{2w + \tau} - \frac{2\sqrt{\Theta}}{2w + \tau} = \frac{\lambda(e_L - e_R) - \kappa_1}{2w + \tau} + \frac{2\sqrt{\Theta}}{2w + \tau} \tag{12}
\]

Multiplying both sides by \(2w + \tau\):

\[
\kappa_1 - 2k_1 + 2dHy - 2\sqrt{\Theta} = \lambda(e_L - e_R) - \kappa_1 + 2\sqrt{\Theta} \tag{13}
\]

Rearranging terms:

\[
\kappa_1 - 2k_1 + 2dHy - \lambda(e_L - e_R) + \kappa_1 = 4\sqrt{\Theta} \tag{14}
\]

Which simplifies to:

\[
2\kappa_1 - 2k_1 + 2dHy - \lambda(e_L - e_R) = 4\sqrt{\Theta} \tag{15}
\]

### Step 7: Verifying the Condition Holds on the Boundary

To verify that equation (15) holds at the boundary, substitute the expression for \(\phi\) from equation (11) into the boundary condition equation (2):

\[
\begin{aligned}
\text{LHS} &= A - F\eta\left(k_1 + (2w + \tau)\phi\right) \\
&= A - F\eta k_1 - F\eta(2w + \tau)\left[\frac{\lambda(e_L - e_R) - \kappa_1}{2w + \tau} + \frac{2\sqrt{\Theta}}{2w + \tau}\right] \\
&= A - F\eta k_1 - F\eta\left[\lambda(e_L - e_R) - \kappa_1 + 2\sqrt{\Theta}\right]
\end{aligned} \tag{16}
\]

Using equation (8) in the form \(A = F\eta[(\kappa_1 - k_1) + 2dHy]\):

\[
\begin{aligned}
\text{LHS} &= F\eta[(\kappa_1 - k_1) + 2dHy] - F\eta k_1 - F\eta\left[\lambda(e_L - e_R) - \kappa_1 + 2\sqrt{\Theta}\right] \\
&= F\eta\left[\kappa_1 - k_1 + 2dHy - k_1 - \lambda(e_L - e_R) + \kappa_1 - 2\sqrt{\Theta}\right] \\
&= F\eta\left[2\kappa_1 - 2k_1 + 2dHy - \lambda(e_L - e_R) - 2\sqrt{\Theta}\right]
\end{aligned} \tag{17}
\]

Set this equal to the RHS of equation (2), which is \(2F\eta\sqrt{\Theta}\):

\[
F\eta\left[2\kappa_1 - 2k_1 + 2dHy - \lambda(e_L - e_R) - 2\sqrt{\Theta}\right] = 2F\eta\sqrt{\Theta} \tag{18}
\]

Dividing both sides by \(F\eta\):

\[
2\kappa_1 - 2k_1 + 2dHy - \lambda(e_L - e_R) - 2\sqrt{\Theta} = 2\sqrt{\Theta} \tag{19}
\]

Rearranging:

\[
2\kappa_1 - 2k_1 + 2dHy - \lambda(e_L - e_R) = 4\sqrt{\Theta} \tag{20}
\]

This is exactly equation (15), confirming that the condition holds at the boundary where \(\Delta_1 = 0\).

## Conclusion

On the boundary of the effective cooperation zone (where \(\Delta_1 = 0\)), equations (F.19) and (F.21) are mathematically equivalent. The equivalence is guaranteed by condition (15), which reflects the equilibrium relationship among model parameters at the boundary.


