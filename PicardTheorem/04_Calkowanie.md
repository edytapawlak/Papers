Zbieżnośc jednostajna a całkowanie

TWIERDZENIE 	\label{tw:calkowanieCiagJednoZb}
Niech $\{f_n(x)\}$ będzie funkcją całkowalną w sensie Riemanna na przedziale $[a,b]$ przy $n = 1, 2, 3, \ldots$ i niech $f_n \rightrightarrows f(x)$ na $[a,b]$.
Wtedy $f$ jest całkowalna i 
	\begin{equation*}
		\int_a^b f dx = \lim_{n \to \infty} \int_a^b f_n dx.
	\end{equation}

DOWÓD.
Niech 
	\begin{equation*}
		\varepsilon_n = \sup_{x \in [a,b]} \left|f_n(x) - f(x) \right|.
	\end{equation*}
Wtedy $f_n - \varepsilon_n \leq f \leq f_n + \varepsilon_n$.
Górne i dolne całki z funkcji $f$ spełniają
	\begin{equation}
		\label{eq:nierCalkiGD}}
		 \int_a^b (f_n - \varepsilon_n) dx \leq \underline{\int f dx} \leq \overline{\int f dx} \leq \int_a^b(f_n+\varepsilon_n) dx}
	\end{equation}
Przekształćmy tę nierówność
	\[\begin{tabular}{cc}
		\int_a^b (f_n - \varepsilon_n) dx \leq \underline{\int f dx} \leq \overline{\int f dx} \leq \int_a^b(f_n+\varepsilon_n) dx} &
		 \big/ - \underline{\int f dx} \\
		 \int_a^b (f_n - \varepsilon_n) dx -  \underline{\int f dx}   \leq 0 \leq \overline{\int f dx} -  \underline{\int f dx} 
		 \leq \int_a^b(f_n+\varepsilon_n) dx} -  \underline{\int f dx}  & 
	\end{tabular}\]
Zauważmy, że $ \int_a^b (f_n - \varepsilon_n) dx -  \underline{\int f dx}   \leq 0$. Zatem mamy
	\begin{equation*}
		 0 \leq \overline{\int f dx} -  \underline{\int f dx} 
		 \leq \int_a^b(f_n+\varepsilon_n) dx} -  \underline{\int f dx} \leq  \int_a^b(f_n+\varepsilon_n) dx} -  \underline{\int f dx} 
		-( \int_a^b (f_n - \varepsilon_n) dx -  \underline{\int f dx}) 
	\end{equation*}

 	\begin{equation*}
		 0 \leq \overline{\int f dx} -  \underline{\int f dx} 
		 \leq 2 \int_a^b\varepsilon_n dx
	\end{equation*} 

	\begin{equation*}
		 0 \leq \overline{\int f dx} -  \underline{\int f dx} 
		 \leq 2 \int_a^b\varepsilon_n dx
	\end{equation*}
 
	\begin{equation*}
		 0 \leq \overline{\int f dx} -  \underline{\int f dx} 
	 	\leq 2 \varepsilon_n \left| b - a \right|
	\end{equation*}
 Ponieważ $\varepsilon_n \to 0$ gdy $n \to \infty$ (patrz rozdział \ref{par:kiedyCiagJestJednZb})
więc całki dolna i górna są równe. Wobec tego $f$ jest całkowalna w sensie Riemanna. 

Wróćmy do nierówności \ref{eq:nierCalkiGD} i przekształćmy ją następująco:
	\begin{equation*}
		\begin{tabular}{cc}
			 \int_a^b (f_n - \varepsilon_n) dx \leq \int f dx  \leq \int_a^b(f_n+\varepsilon_n) dx}
			& \big/ - \int_a^b( f_n - \varepsilon) dx \\
			0  \leq \int f dx -  \int_a^b f_n - \int^b_a \varepsilon_n dx \leq 2 \int_a^b \varepsilon_n dx & \\
			0  \leq \int f dx -  \int_a^b f_na \leq  \int_a^b \varepsilon_n dx & \\
			\left| \int f dx -  \int_a^b f_n\right|  \leq  \int_a^b \varepsilon_n dx & \\
			\left| \int f dx -  \int_a^b f_n\right|  \leq \varepsilon_n \left| b - a \right| & 
		\end{tabular}
	\end{equation*}
	
co oznacza, że 
	\begin{equation*}
		\int_a^b f dx = \lim_{n \to \infty} \int_a^b f_n dx.
	\end{equation*}


