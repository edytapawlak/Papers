DEF. \label{def:zbieznoscpunktowa}} (Zbieżność punktowa) Niech\(\{f_n\}, n= 1, 2, 3, /ldots\), będzie ciągiem funkcji określonym na zbiorze \(E\) i niech ciąg liczb \(\{f_n(x)\}\) będzie zbieżny dla każdego \(x \in E\). Możemy wtedy określić funkcję \(f\) jako 
	\[f(x) = \lim_{n \to \infty} f_n(x), \quad (x \in E).\]
W tym przypadku powiemy, że ciąg \(\{f_n\}\)jest zbieżny na zbiorze \(E\) i funkcja \(f\) jest granicą lub funkcją graniczną tego ciągu. 
Analogicznie jeśli szereg \(\sum f_n(x)\) jest zbieżny przy każdym \(x \in E\), to określimy
	\[f(x) = \sum^{\infty}_{n=1} f_n(x) \quad (x \in E)\]
i funkcję \(f\) nazywać będziemy sumą szeregu \(\sum f_n(x)\).

Przypomnijmy, ze szereg jest zbieżny, gdy zbieżny jest ciąg jego sum częściowych, a granicę tego ciągu nazywamy sumą szeregu.

Czy granica ciągu funkcyjnego jest funkcją ciągłą?

Nie, co pokazuje przykład.
PRZYKŁAD. \label{ex1:zbieznoscpunktowa}}
Niech \(x=[0,1] \subset \mathbb{R}\) i niech \(f_n: [0,1] \to \mathbb{R}\) będzie dana wzorem \(f_n(x) = x^n\).
Wtedy
	\[\lim_{n \in \infty} f_n(x) = \lim_{n \to \infty} x^n = f(x) = 
	\begin{cases} 
	0, \quad x \in [0,1) \\
	1, \quad x = 1\]
Zatem ciąg, którego elementami są funkcje ciągłe, może być zbieżny do funkcji nieciągłej.

Ciągłość funkcji w punkcie \(x\) oznacza,że 
	\[\lim_{t \to x} f(t) = f(x)\]
Zatem czy zachodzi równość
	\[\lim_{t \to x} \lim_{n \to \infty} f_n(t) = \lim_{n \to \infty} \lim_{t \to x} f_n(t)\]?
Czy istotna jest kolejnośc w jakiej dokonuje się przejść granicznych?

PRZYKŁAD \label{ex2:zbieznoscpunktpowa}}
Określmy przy \(m = 1, 2, 3,\ldots\) i \(n = 1, 2, 3,\ldots\)
	\[s_{nm} = \frac{m}{n+m}\]
Wtedy dla ustalonego \(n\) \(\lim_{m \to \infty} s_{nm}=1\), czyli
\[\lim_{n\to \infty}\lim_{m \to \infty} s_{nm}=1\]
Z drugiej strony, przy dowolnym ustalonym \(m\) \(\lim_{n \to \infty} s_{nm}=0)\, zatem
\[\lim_{m\to \infty}\lim_{n \to \infty} s_{nm}=-0\]


DEF. \label{def:zbieznoscjednostajna} (Zbieżność jednostajna)
Powiemy, że ciąg funkcji \(\{f_n\}\) jest zbieżny jednostajnie na zbiorze \(E\) do funkcji \(f\), jeżeli dla dowolnego \(\varepsilon >0 \) istnieje liczba naturalna \(N\) taka, że dla \(n \leq N\) zachodzi 
	\[\left| f_n(x) - f(x) \right| \leq \varepsilon\] 
przy dowolnym \(x \in E\).

Powiemy, że szereg \(\sum f_n(x)) jest na zbiorze E zbieżny jednostajnie, jeżeli ciąg \{s_n\} sum częściowych określonych równością 
	\[s_n(x) = \sum^{n}_{i=1} f_i(x)\]
jest zbieżny jednostajnie na zbiorze E.

Jaka jest różnica między zbieżnością punktową a jednostajną?
Zapiszmy definicje używając kwantyfikatorów

Zbieżnośc punktowa \(f_n \to f\) na \(E\):\( \forall x \in E \forall \varepsilon>0 \exists N = N(x, \varepsilon)>0 \forall n>0 (\left|f_n(x)-f(x)\right|<\varepsilon). \)
Zbieżnośc jednostajna \(f_n \to \rightrightarrows f\) na \(E\)  \forall \varepsilon>0 \exists N = N(\varepsilon)>0 \forall x \in E \forall n>0 (\left|f_n(x)-f(x)\right|<\varepsilon).

Ciąg zbieżny jednostajnie jest także zbieżny punktowo. Różnica polega na tym, ze przy zbieżności punktowej liczbę \(N\) wybieramy mając już ustalone \(x\) i \(\varepsilon\), zatem \(N\) jest zależne od \(x\) i \(\varepsilon\).
Jeżeli ciąg jest zbieżny jednostajnie, to przy każdym \(\varepsilon>0\) można dobrać jedną wspólną dla wszystkich punktów \(x \in E\) liczbę \(N\).

Wróćmy do przykładu ref{ex1:zbieznoscpunktowa}  i pokażmy, że ciąg \(\{f_n\}\) nie jest zbieżny jednostajnie. Przypomnijmy, że
	\(X=[0,1]\), \(x \in X\),
	f_n(x)=x^n \\
	f(x) = 
	\begin{cases} 
	0, \quad x \in [0,1) \\
	1, \quad x = 1\]
Zauważmy, że dla \(x = 2^{-frac{1}{n}}\) mamy:
\[f_n(x)- f(x) = f_n( 2^{-frac{1}{n}}) - f( 2^{-frac{1}{n}}) = \frac{1}{2}\]
Zatem warunek jednostajnej zbieżności nie zachodzi dla \(\varepsilon < \frac{1}{2}\).

