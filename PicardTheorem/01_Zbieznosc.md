DEF. \label{def:zbieznoscpunktowa}} (Zbieżność punktowa) Niech$\{f_n\}, n= 1, 2, 3, /ldots$, będzie ciągiem funkcji określonym na zbiorze \(E\) i niech ciąg liczb $\{f_n(x)\}$ będzie zbieżny dla każdego $x \in E$. Możemy wtedy określić funkcję $f$ jako 
	\begin{equation}
		f(x) = \lim_{n \to \infty} f_n(x), \quad (x \in E).
	\end{equation}
W tym przypadku powiemy, że ciąg $\{f_n\}$jest zbieżny na zbiorze $E$ i funkcja $f$ jest granicą lub funkcją graniczną tego ciągu. 
Analogicznie jeśli szereg $\sum f_n(x)$ jest zbieżny przy każdym $x \in E$, to określimy
	\begin{equation}
		f(x) = \sum^{\infty}_{n=1} f_n(x) \quad (x \in E)
	\end{equation}
i funkcję $f$ nazywać będziemy sumą szeregu $\sum f_n(x)$.

Przypomnijmy, ze szereg jest zbieżny, gdy zbieżny jest ciąg jego sum częściowych, a granicę tego ciągu nazywamy sumą szeregu.

Czy granica ciągu funkcyjnego jest funkcją ciągłą?

Nie, co pokazuje przykład.
PRZYKŁAD. \label{ex1:zbieznoscpunktowa}}
Niech $x=[0,1] \subset \mathbb{R}$ i niech $f_n: [0,1] \to \mathbb{R}$ będzie dana wzorem $f_n(x) = x^n$.
Wtedy
	\begin{equation} 
		\lim_{n \in \infty} f_n(x) = \lim_{n \to \infty} x^n = f(x) = 
		\begin{cases} 
			0, \quad x \in [0,1) \\
			1, \quad x = 1
	\end{equation}]
Zatem ciąg, którego elementami są funkcje ciągłe, może być zbieżny do funkcji nieciągłej.

Ciągłość funkcji w punkcie $x$ oznacza,że 
	\begin{equation} 
		\lim_{t \to x} f(t) = f(x)
	\end{equation}
Zatem czy zachodzi równość
	\begin{equation}
		\lim_{t \to x} \lim_{n \to \infty} f_n(t) = \lim_{n \to \infty} \lim_{t \to x} f_n(t) 
	\end{equation}?
Czy istotna jest kolejnośc w jakiej dokonuje się przejść granicznych?

PRZYKŁAD \label{ex2:zbieznoscpunktpowa}}
Określmy przy $m = 1, 2, 3,\ldots$ i $n = 1, 2, 3,\ldots$
	\begin{equation}
		s_{nm} = \frac{m}{n+m}
	\end{equation}
Wtedy dla ustalonego $n$ $\lim_{m \to \infty} s_{nm}=1$, czyli
	\begin{equation}
		\lim_{n\to \infty}\lim_{m \to \infty} s_{nm}=1
	\end{equation}
Z drugiej strony, przy dowolnym ustalonym $m$ $\lim_{n \to \infty} s_{nm}=0$, zatem
	\begin{equation}
		\lim_{m\to \infty}\lim_{n \to \infty} s_{nm}=-0
	\end{equation}


