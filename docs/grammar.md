# Grammar

**Warning:** This doesn't work on GitHub. If you want to see it, you will have to open this file in ***Visual Studio Code*** or any other text editor that supports ***Math Mode***.

$$
\begin{align}
[\text{Prog}] &\to [\text{Stmt}]^* \\
[\text{Stmt}] &\to
\begin{cases}
\text{exit}([\text{Expr}]); \\
\text{let}\space\text{ident} = [\text{Expr}];
\end{cases} \\
[\text{Expr}] &\to
\begin{cases}
\text{[Term]} \\
[\text{BinExpr}]
\end{cases} \\
[\text{BinExpr}] &\to
\begin{cases}
[\text{Expr}] * [\text{Expr}] & \text{prec} = 1 \\
[\text{Expr}] / [\text{Expr}] & \text{prec} = 1 \\
[\text{Expr}] + [\text{Expr}] & \text{prec} = 0 \\
[\text{Expr}] - [\text{Expr}] & \text{prec} = 0 \\
\end{cases} \\
[\text{Term}] &\to
\begin{cases}
\text{int\_lit} \\
\text{ident} \\
([\text{Expr}])
\end{cases}
\end{align}
$$
