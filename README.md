Denotaremos s1[0..j] uma subpalavra de s1 do caractere 0 até o carectere j. Seja LCS(s1[0..j], s2[0..k]) depende de:

\begin{itemize}
\item se s1[j] == s2[k] então esse caractere está na maior subsequência comum e podemos resolver o problema LCS(s1[0..j-1], s2[0..k-1])
\item se s1[j] != s2[k] então precisamos resolver LCS(s1[0..j-1], s2[0..k]) e LCS(s1[0..j], s2[0..k-1])
\end{itemize}
