📊 Production Trend Analysis using Quadratic Polynomial & Newton-Raphson Method
📌 Project Overview

This project analyzes monthly production data (2018–2023) using a quadratic polynomial regression model. The goal is to capture non-linear production trends and make future predictions, including estimating when production will exceed warehouse capacity.

The implementation covers:

Quadratic polynomial regression via Least Squares (Normal Equation & Pseudoinverse).

Validation of polynomial accuracy using the Taylor Series approximation.

Forecasting critical capacity exceedance using the Newton-Raphson method.

⚙️ Features

Quadratic Polynomial Regression

Captures both linear and non-linear trends in production.

Computed using Normal Equation and Pseudoinverse (both yield identical results).

Taylor Series Verification

Demonstrates that the quadratic model perfectly matches the Taylor Series expansion (since it’s a degree-2 polynomial).

Newton-Raphson Forecasting

Predicts when production exceeds the 25,000-bag warehouse capacity.

Accurately identifies the optimal month to start building a new warehouse.

📈 Methods & Equations

Quadratic Model:

𝑓
(
𝑥
)
=
𝑎
𝑥
2
+
𝑏
𝑥
+
𝑐
f(x)=ax
2
+bx+c

Normal Equation:

𝑎
=
(
𝐴
𝑇
𝐴
)
−
1
𝐴
𝑇
𝑌
a=(A
T
A)
−1
A
T
Y

Pseudoinverse Method:

𝑎
=
𝐴
+
𝑌
a=A
+
Y

Newton-Raphson Iteration:

𝑥
𝑛
+
1
=
𝑥
𝑛
−
𝑓
(
𝑥
𝑛
)
𝑓
′
(
𝑥
𝑛
)
x
n+1
	​

=x
n
	​

−
f
′
(x
n
	​

)
f(x
n
	​

)
	​

