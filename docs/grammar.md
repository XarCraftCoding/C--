# Grammar

**Warning:** This doesn't work on GitHub. If you want to see it, you will have to open this file in **_Visual Studio Code_** or any other text editor that supports **_Math Mode_**.

$$
\begin{align}
[\text{Prog}] &\to [\text{Stmt}]^* \\
[\text{Stmt}] &\to
\begin{cases}
\text{exit}([\text{Expr}]); \\
\text{let}\space\text{ident} = [\text{Expr}]; \\
\{[\text{Stmt}]^*\}
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
