% ============================================================
%  MATH161: Engineering Calculus — Final Project
%  Ashesi University, Spring 2026
% ============================================================
 
\documentclass[12pt]{article}
 
% ---------- Essential packages only ----------
\usepackage[margin=1in]{geometry}
\usepackage{amsmath, amssymb}
\usepackage{graphicx}
\usepackage{setspace}
\usepackage{parskip}
\usepackage{hyperref}
\usepackage{booktabs}   % for clean tables (Riemann sums table)
 
% ---------- Hyperlink style ----------
\hypersetup{
    colorlinks=true,
    linkcolor=black,
    urlcolor=black,
    citecolor=black
}
 
% ---------- Line spacing ----------
\onehalfspacing
 
% ============================================================
\begin{document}
 
% ============================================================
%  TITLE PAGE
% ============================================================
\begin{titlepage}
    \centering
    \vspace*{2cm}
 
    {\Large \textbf{Ashesi University}}\\[0.4cm]
    {\large Department of Mathematics}\\[0.4cm]
    {\large Spring 2026}\\[1.5cm]
 
    \rule{\linewidth}{0.5pt}\\[0.4cm]
    {\LARGE \textbf{MATH161: Engineering Calculus}}\\[0.3cm]
    {\Large \textbf{Final Project}}\\[0.2cm]
    \rule{\linewidth}{0.5pt}\\[2cm]
 
    \begin{tabular}{ll}
        \textbf{Student Name:}  & Clement Agyakwah Somuah     \\[0.3cm]
        \textbf{Student ID:}    & 39972029 
        \\[0.3cm]
        \textbf{Student Name:}  & Mathew Kobby Konadu
        \\[0.3cm]
        \textbf{Student ID:}    & 73082029 
        \\[0.3cm]
         \textbf{Student Name:}  & Abigeal Seifu Adamssu    
        \\[0.3cm]
         \textbf{Student ID:}    & 06912029
        \\[0.3cm]
        \textbf{Instructor:}    & Dr. Patrick Dwomfuor        \\[0.3cm]
        \textbf{Submission Date:} & Thursday, 23rd April 2026 \\
    \end{tabular}
 
  
\end{titlepage}


















 
% ============================================================
%  ABSTRACT
% ============================================================
\newpage
\begin{abstract}
\noindent

This project explores important concepts in engineering calculus, including derivatives, continuity, Riemann sums, definite integrals and applications like volume of solids and area between curves. The goal of the project is to build relationship between functions and their derivative, examine conditions for continuity and differentiability and demonstrate how integration can be used to approximate and calculate exact values

GeoGebra was used as the primary tool for graphical visual and numerical approximation across all activities. Activity 1, the relationship between a function and its first and second derivatives was analyzed through graphical interpretation. Activity 2 which is continuity and differentiability, showing that differentiability implies continuity but not vice versa. Activity 3 explored the connection between Riemann sums and definite integrals, showing that as the number of rectangles increases the approximation approaches the exact value. Activity 4 focused on practical application of interaction, including the calculation of volume of solids of revolution and the area between curves. 

\end{abstract}










 
% ============================================================
%  TABLE OF CONTENTS
% ============================================================
\newpage
\tableofcontents








 
% ============================================================
%  ACKNOWLEDGEMENT
% ============================================================
\newpage
\section*{Acknowledgement}
\addcontentsline{toc}{section}{Acknowledgement}
 
We would like to express our sincere gratitude to our Engineering Calculus Faculty for constantly encouraging us to go beyond our comfort zone to get solutions to problems. We are grateful to the Ashesi Writing Center, also, for helping us refine our texts and exposing us to better ways of expressing ourselves. We're grateful to our seniors and friends who stepped up to help us use tools to put this piece together. 



 
% ============================================================
%  GENERAL INTRODUCTION
% ============================================================
\newpage
\section{General Introduction}
 
Calculus is a branch of mathematics that helps us understand change and how things add up over time. It mainly focuses on function, derivatives, and integrals, A function shows how two variables are related. Derivatives help us understand how fast something is changing while integrals help find total amounts such as area, volume or accumulated change.
In real life, calculus is used in many areas of science and engineering. For example, in physics, derivatives are used to calculate velocity and acceleration. If a car is moving, its speed at a specific moment is found using derivatives. Integrals are used to calculate the total distance the car travels over time. In engineering, calculus is used when designing structures like bridges and buildings to make sure they are safe and stable. Engineers also use integrals to calculate the volume of materials needed, such as concrete for construction.
Another example is in medicine, where calculus is used to model how drugs move through the body over time. In economics, it is used to find maximum profit and minimum cost. These examples show that calculus is not just theory but is very useful in solving real-world problems.
In this project, these concepts are explored using graphs, calculations, and GeoGebra. The point is to understand how derivatives and integrals work and how they can be applied to solve practical problems.


















% ============================================================
%  ACTIVITY 1: Functions and Their Derivatives
% ============================================================
\newpage
\section{Activity 1: Functions and Their Derivatives}

\subsection{Introduction}
This activity explores the relationship between a function and the graphs of its first and second derivatives. We investigate these relationships using $f(x) = x^2 e^{-x}$ and verify our conjectures with $g(x) = x^3 + 4x + 2$.

\subsection{Methodology}
To perform this analysis, the following steps were taken in GeoGebra:
\begin{enumerate}
    \item \textbf{Function Definition:} The function $f(x) = x^2 e^{-x}$ was entered into the input bar.
    \item \textbf{Differentiation:} The first derivative $f'(x)$ and second derivative $f''(x)$ were generated using the \texttt{f'(x)} and \texttt{f''(x)} commands.
    \item \textbf{Critical Point Identification:} The \texttt{Roots} and \texttt{Intersect} tools were used to find the exact x-values where $f'(x)=0$ and $f''(x)=0$.
    \item \textbf{Visualization:} To compare behaviors, side-by-side axes were created. One axis displayed $f(x)$ and $f'(x)$, while the other displayed $f(x)$ and $f''(x)$.
    \item \textbf{Verification:} The same process was repeated for $g(x) = x^3 + 4x + 2$ to verify the established conjectures.
\end{enumerate}

\subsection{Calculus Derivations}

\subsubsection*{Part (i) — First Derivative of $f(x) = x^2 e^{-x}$}
To find $f'(x)$, we apply the Product Rule: $\frac{d}{dx}[uv] = u'v + uv'$.
Let $u = x^2 \implies u' = 2x$.
Let $v = e^{-x} \implies v' = -e^{-x}$ (by the Chain Rule).
\begin{align*}
    f'(x) &= (2x)(e^{-x}) + (x^2)(-e^{-x}) \\
    &= 2xe^{-x} - x^2e^{-x} \\
    &= x(2 - x)e^{-x}
\end{align*}

\subsubsection*{Step-by-Step Second Derivative}
To find $f''(x)$, we differentiate $f'(x) = (2x - x^2)e^{-x}$ using the Product Rule again.
Let $u = 2x - x^2 \implies u' = 2 - 2x$.
Let $v = e^{-x} \implies v' = -e^{-x}$.
\begin{align*}
    f''(x) &= (2 - 2x)(e^{-x}) + (2x - x^2)(-e^{-x}) \\
    &= e^{-x} (2 - 2x - 2x + x^2) \\
    &= (x^2 - 4x + 2)e^{-x}
\end{align*}

\subsubsection*{Part (ii) — Side-by-Side Graphs}
\begin{figure}[h!]
    \centering
    \begin{minipage}{0.48\textwidth}
        \centering
        \includegraphics[width=\textwidth]{ACTIVITY_1_GRAPH_2.png}
        \caption{$f(x)$ (green) and $f'(x)$ (blue)}
    \end{minipage}
    \hfill
    \begin{minipage}{0.48\textwidth}
        \centering
        \includegraphics[width=\textwidth]{ACTIVITY_1_GRAH_3.png}
        \caption{$f(x)$ (green) and $f''(x)$ (grey)}
    \end{minipage}
\end{figure}

\subsection{Results}

\subsubsection*{Part (iii) — Zeros and Sign of $f'(x)$}
The first derivative $f'(x) = x(2-x)e^{-x}$ equals zero at $x = 0$ and $x = 2$. 
\begin{itemize}
    \item $f'(x) > 0$ on $(0, 2)$: The blue curve is above the x-axis, justifying that $f(x)$ is increasing.
    \item $f'(x) < 0$ on $(-\infty, 0) \cup (2, \infty)$: The blue curve is below the x-axis, justifying that $f(x)$ is decreasing.
\end{itemize}

\subsubsection*{Part (iv) — Zeros and Sign of $f''(x)$}
Solving $x^2 - 4x + 2 = 0$ via the quadratic formula gives $x = 2 \pm \sqrt{2}$, or $x \approx 0.586$ and $x \approx 3.414$.
\begin{itemize}
    \item $f''(x) > 0$ on $(-\infty, 0.586) \cup (3.414, \infty)$: The grey curve is above the x-axis, indicating concave up.
    \item $f''(x) < 0$ on $(0.586, 3.414)$: The grey curve is below the x-axis, indicating concave down.
\end{itemize}

\subsection{Discussion}

\subsubsection*{Part (v) — Monotonicity Conjecture}
\textbf{Conjecture:} A function $f(x)$ increases when $f'(x) > 0$, decreases when $f'(x) < 0$, and is stationary when $f'(x) = 0$. This holds true for all differentiable functions as the derivative represents the instantaneous rate of change.

\subsubsection*{Part (vi) — Verification with $g(x)$}
For $g(x) = x^3 + 4x + 2$, the derivative is $g'(x) = 3x^2 + 4$. Since $x^2$ is always non-negative, $3x^2 + 4$ is always $\geq 4$. Thus, $g'(x) > 0$ for all $x$, and the graph of $g(x)$ is strictly increasing.

\subsubsection*{Part (vii) — Concavity Conjecture}
\textbf{Conjecture:} The sign of the second derivative determines concavity. $f(x)$ is concave up where $f''(x) > 0$ and concave down where $f''(x) < 0$.

\subsubsection*{Part (viii) — Verification with $g''(x)$}
For $g(x)$, $g''(x) = 6x$. $g''(x) < 0$ for $x < 0$ and $g''(x) > 0$ for $x > 0$, aligning with the observed inflection point at the origin for cubic functions.


















% ============================================================
%  ACTIVITY 2: Continuity and Differentiability
% ============================================================
\newpage
\section{Activity 2: Continuity and Differentiability}

\subsection{Introduction}
This activity explores the concepts of continuity and derivatives and investigates the relationship between them. We analyze whether a function is differentiable at a point where it is discontinuous or where it is continuous but has a sharp change in direction[cite: 27, 28].

\subsection{Methodology}
I utilized GeoGebra to graph $f(x) = \frac{x-3}{\sqrt{x^2-9}}$ and developed applets to test behavior at $x=1$ and $x=3$. A tabular approach was used in the Spreadsheet view to observe limits, while a graphical approach using the difference quotient was used to establish the existence of derivatives.

\subsection{Results}

\subsubsection*{Part (i) — Global Graph of the Function}
The function was plotted to identify its domain and overall behavior.

\begin{figure}[h!]
    \centering
    \includegraphics[width=0.75\textwidth]{Activity 2 (a)(i).png}
    \caption{Global graph of $f(x)$ showing the domain $(-\infty, -3) \cup (3, \infty)$[cite: 24].}
\end{figure}

\subsubsection*{Part (ii) — Continuity Applet (Graphical and Tabular)}
 


    \hfill
    \begin{table}[h]
\centering
\begin{minipage}{0.45\textwidth}
    \centering
    \begin{tabular}{|c|c|}
        \hline
        $x$ & $f(x)$ \\ \hline
        3.5   & 0.2773 \\ \hline
        3.1   & 0.1280 \\ \hline
        3.01  & 0.0408 \\ \hline
        3.001 & 0.0041 \\ \hline
        \textbf{3.0} & \textbf{Undefined} \\ \hline
    \end{tabular}
    \caption*{Table 1: Values of $f(x)$ near $x = 3$}
\end{minipage}
\end{table}


\textbf{Findings:} The function is discontinuous at $x=1$ and $x=3$ because it is undefined at those points.

\subsubsection*{Part (iii) — Differentiability Applet}
A second applet was used to check the existence of the derivative using the limit of the difference quotient.

\begin{figure}[h!]
    \centering
    \includegraphics[width=0.6\textwidth]{Act3.png} 
    \caption{Applet testing the derivative $\lim_{h \to 0} \frac{f(x+h)-f(x)}{h}$.}
\end{figure}

\subsection{Discussion}

\section*{iv) Derivative at a Point of Discontinuity}

Based on the results from parts (ii) and (iii) for $f(x) = \dfrac{x-3}{\sqrt{x^2-9}}$, the function is
discontinuous at $x = 3$ (the expression is undefined there), and the derivative at $x = 3$ was
also found not to exist.

This leads to the following conclusion:

\begin{theorem}
If $f$ is not continuous at $x = a$, then $f$ is not differentiable at $x = a$.
\end{theorem}

\begin{proof}
The derivative of $f$ at $x = a$ is defined as:
\[
    f'(a) = \lim_{h \to 0} \frac{f(a+h) - f(a)}{h}
\]
For this limit to exist, $f(a)$ must itself be defined, and $f$ must be continuous at $x = a$.
If $f$ is discontinuous at $x = a$, then either $f(a)$ is undefined, or
$\lim_{x \to a} f(x) \neq f(a)$, in either case making the difference quotient ill-defined.
Therefore, the derivative cannot exist at a point of discontinuity.
\end{proof}

\noindent\textbf{Conclusion:} The derivative of a function at a point of discontinuity does \textbf{not} exist.


\section*{v) Differentiability at a Point of Continuity}

Using the results from parts (ii) and (iii), continuity at a point is \emph{necessary} but
\textbf{not sufficient} for differentiability. That is:
\[
    f \text{ differentiable at } a \implies f \text{ continuous at } a,
    \qquad \text{but the converse is } \textbf{false}.
\]

\subsection*{Check: $y = |x|$ at $x = 0$}

\textbf{Continuity:}
\[
    \lim_{x \to 0} |x| = 0 = f(0)
\]
So $y = |x|$ is continuous at $x = 0$. 

\bigskip
\textbf{Differentiability:}

Left-hand derivative:
\[
    \lim_{h \to 0^-} \frac{|0 + h| - |0|}{h} = \lim_{h \to 0^-} \frac{-h}{h} = -1
\]

Right-hand derivative:
\[
    \lim_{h \to 0^+} \frac{|0 + h| - |0|}{h} = \lim_{h \to 0^+} \frac{h}{h} = +1
\]

Since the left-hand and right-hand derivatives are not equal:
\[
    \lim_{h \to 0^-} \frac{|h|}{h} \neq \lim_{h \to 0^+} \frac{|h|}{h}
\]
the derivative of $y = |x|$ at $x = 0$ does \textbf{not} exist, even though the function is
continuous there.

\subsection*{Summary}


\noindent\textbf{Conclusion:} Differentiability is a strictly stronger condition than continuity.
A function can be continuous at a point without being differentiable there, as demonstrated by
$y = |x|$ at $x = 0$.


% ============================================================
%  ACTIVITY 3: Riemann Sums and Definite Integration
% ============================================================
\newpage
\section{Activity 3: Riemann Sums and Definite Integration}

\subsection{Introduction}
Before the formal definition of the integral existed, mathematicians approximated areas under curves by filling them with rectangles. This idea, formalised by Bernhard Riemann, forms the bridge between geometry and the algebraic definition of the definite integral.

\subsection{Methodology}
The following procedures were executed in GeoGebra to perform the analysis:
\begin{enumerate}
    \item \textbf{Function Plotting:} The function $f(x) = x^{2}+2$ was defined over the interval $[0,2]$.
    \item \textbf{Slider Implementation:} A slider \texttt{n} was created (range 1 to 10,000) to represent the number of sub-intervals.
    \item \textbf{Riemann Sum Calculation:} The \texttt{RectangleSum(f, 0, 2, n, 1)} command was utilized to compute the right-endpoint sum $R_n$.
    \item \textbf{Verification:} The \texttt{Integral(f, 0, 2)} command provided the analytical exact value for comparison.
\end{enumerate}

\subsection{Results and Discussion}

\subsubsection*{Part (i) — Graphical Representation}
The parabola $y=x^{2}+2$ is an upward-opening parabola shifted up by 2 units. On $[0,2]$, it rises from $y=2$ at $x=0$ to $y=6$ at $x=2$.

% This minipage block prevents LaTeX from separating the image and table
\begin{minipage}{\textwidth}
    \centering
    \includegraphics[width=0.55\textwidth]{Act4.png}
    \captionof{figure}{The region under $y=x^2+2$ on $[0,2]$ approximated by rectangles.}
    \label{fig:act3graph}
    \vspace{0.3em} % Adds a small space between image and table

    \captionof{table}{Right-endpoint Riemann sums $R_{n}$ for $y=x^{2}+2$ on $[0,2]$}
    \begin{tabular}{cc}
    \toprule
    $n$ & $R_{n}\midrule
    10  & 7.0800  \\ 
    20  & 6.8700  \\
    30  & 6.8015 \\ 
    60  & 6.7337 \\ \bottomrule
    \end{tabular}
\end{minipage}

\subsubsection*{Part (ii) — Riemann Sum Formula}
Using the right-endpoint rule with $n$ equal sub-intervals ($\Delta x = 2/n$):
\[
R_{n} = \sum_{k=1}^{n}\left[\left(\frac{2k}{n}\right)^{2}+2\right]\frac{2}{n} = \frac{4(n+1)(2n+1)}{3n^{2}}+4.
\]

\subsubsection*{Part (iii) — Definite Integral and Conclusion}
The exact area is calculated analytically as follows:
\begin{align*}
\int_{0}^{2}(x^{2}+2)\,dx &= \left[\frac{x^{3}}{3}+2x\right]_{0}^{2} \\
&= \left(\frac{8}{3} + 4\right) - 0 = \frac{20}{3} \approx 6.6667
\end{align*}

\textbf{Conclusion:} As $n \to \infty$, the Riemann sum $R_n$ converges to $20/3$. This establishes that the definite integral is exactly the limit of the Riemann sums.














% ============================================================
%  ACTIVITY 4: Volumes of Revolution and Areas Between Curves
% ============================================================
\newpage
\section{Activity 4: Volumes of Revolution and Areas Between Curves}

\subsection{Introduction}
This activity applies integration to compute the volume of solids formed by revolving functions about the x-axis and determines the area between curves. By comparing individual geometric properties to bounded regions, we establish fundamental relations used in engineering design and spatial modeling.

\subsection{Methodology}
The following technical procedures were executed in GeoGebra to perform the geometric analysis:

\subsubsection*{Part (a): Volume of Revolution via Washer Method}
\begin{enumerate}
    \item \textbf{Function Definition:} Input $f(x) = x^{1/3}$ and $g(x) = x/4$ to define the boundary curves.
    \item \textbf{Interval Determination:} Used the \texttt{Intersect} tool to confirm the limits of integration at $x=0$ and $x=8$.
    \item \textbf{Volume Extraction:} Individual volumes were computed using the disk method formula via the commands \texttt{Integral[pi * f\textasciicircum2, 0, 8]} and \texttt{Integral[pi * g\textasciicircum2, 0, 8]}.
    \item \textbf{Washer Method Implementation:} Calculated the final volume of the bounded solid using \texttt{Integral[pi * (f\textasciicircum2 - g\textasciicircum2), 0, 8]}, which subtracts the inner volume from the outer volume.
\end{enumerate}

\subsubsection*{Part (b): Area Analysis via Integration}
\begin{enumerate}
    \item \textbf{Curve Plotting:} Defined $f(x) = x e^{-x^2}$ and $g(x) = x+1$ within the GeoGebra Algebra view.
    \item \textbf{Constraint Definition:} Plotted vertical lines $x=0$ and $x=2$ to set the boundaries for the definite integral.
    \item \textbf{Area Computation:} Utilized \texttt{Integral[f, 0, 2]} and \texttt{Integral[g, 0, 2]} to find individual areas under the curves.
    \item \textbf{Bounded Region Evaluation:} Applied the \texttt{IntegralBetween[g, f, 0, 2]} command to find the precise area enclosed by the two functions.
\end{enumerate}

\subsection{Part (a): Volumes of Revolution — $y = \sqrt[3]{x}$ and $y = \frac{x}{4}$}

\subsubsection*{Part (a-i) \& (a-ii) — Side-by-Side Individual Graphs}
The functions $y=\sqrt[3]{x}$ and $y=\frac{x}{4}$ were graphed on separate axes to visualize the functions individually for the interval $0 \le x \le 8$.

\begin{figure}[h!]
    \centering
    \begin{minipage}{0.48\textwidth}
        \centering
        \includegraphics[width=\textwidth]{activity4a1.pdf}
        \caption{$y = \sqrt[3]{x}$}
    \end{minipage}
    \hfill
    \begin{minipage}{0.48\textwidth}
        \centering
        \includegraphics[width=\textwidth]{activity4a2.pdf}
        \caption{$y = \frac{x}{4}$}
    \end{minipage}
\end{figure}

The individual volumes are derived as follows:
\begin{align*}
    V_1 &= \pi \int_0^8 (x^{1/3})^2 dx = \pi \int_0^8 x^{2/3} dx = \pi \left[ \frac{3}{5}x^{5/3} \right]_0^8 = \frac{96\pi}{5} \\
    V_2 &= \pi \int_0^8 \left(\frac{x}{4}\right)^2 dx = \frac{\pi}{16} \int_0^8 x^2 dx = \frac{\pi}{16} \left[ \frac{x^3}{3} \right]_0^8 = \frac{32\pi}{3}
\end{align*}

\subsubsection*{Part (a-iii) — Combined Graph and Bounded Volume}
\begin{figure}[h!]
    \centering
    \includegraphics[width=0.6\textwidth]{activity4a3.pdf}
    \caption{Combined graph of $y = \sqrt[3]{x}$ and $y = \frac{x}{4}$ on $[0,8]$.}
\end{figure}

Using the washer method, the volume is:
\begin{equation*}
    V = \pi \int_0^8 \left( (x^{1/3})^2 - \left(\frac{x}{4}\right)^2 \right) dx = V_1 - V_2 = \frac{128\pi}{15}
\end{equation*}

\subsubsection*{Part (a-iv) — Established Relation}
The results confirm that the volume of the bounded solid is obtained by the relation $V = V_{outer} - V_{inner}$.

\subsection{Part (b): Area Between Curves — $y = xe^{-x^2}$ and $y = x+1$}

\subsubsection*{Part (b-i) \& (b-ii) — Side-by-Side Individual Graphs}
\begin{figure}[h!]
    \centering
    \begin{minipage}{0.48\textwidth}
        \centering
        \includegraphics[width=\textwidth]{activity4b2.pdf}
        \caption{$y = xe^{-x^2}$}
    \end{minipage}
    \hfill
    \begin{minipage}{0.48\textwidth}
        \centering
        \includegraphics[width=\textwidth]{activity4b3.pdf}
        \caption{$y = x+1$}
    \end{minipage}
\end{figure}

Analytical area calculations:
\begin{align*}
    A_1 &= \int_0^2 xe^{-x^2} dx = \frac{1}{2} [e^u]_{-4}^0 = \frac{1 - e^{-4}}{2} \approx 0.491 \\
    A_2 &= \int_0^2 (x+1) dx = \left[ \frac{x^2}{2} + x \right]_0^2 = 4
\end{align*}

\subsubsection*{Part (b-iii) — Combined Graph and Bounded Area}
\begin{figure}[h!]
    \centering
    \includegraphics[width=0.6\textwidth]{activity4b1.pdf} 
    \caption{Region bounded by $y = xe^{-x^2}$ and $y = x+1$ on $[0,2]$.}
\end{figure}

The total area of the bounded region is:
\begin{equation*}
    A = \int_0^2 ((x+1) - xe^{-x^2}) dx = A_2 - A_1 = 3.509
\end{equation*}

\subsubsection*{Part (b-iv) — Established Relation}
The area of the bounded region is established as the difference between the areas of the upper and lower functions: $A = A_{upper} - A_{lower}$.
% ============================================================
%  GENERAL CONCLUSION
% ============================================================
\newpage
\section{General Conclusion}

In conclusion, this project has shown the importance of calculus in analyzing functions, understanding rates of change, and calculating accumulated quantities. The use of derivatives helped explain the behavior of functions while integrals provided accurate methods for determining area and volumes. The connection between Riemann sums and definite integrals was clearly established, showing how approximation approaches exact values.

\subsection*{Key Lessons Learnt}
\begin{itemize}
    \item Derivatives are essential for characterizing function behavior, specifically monotonicity and concavity.
    \item Integrals provide rigorous methods for calculating areas and volumes that are vital in engineering applications.
    \item Riemann sums serve as a fundamental bridge between discrete approximations and exact continuous accumulation.
\end{itemize}

\subsection*{Challenges and Limitations}
One of the challenges encountered was ensuring accuracy in graphical representations and numerical approximations, particularly when transitioning between manual calculations and GeoGebra outputs. Regardless of these challenges, the project provided valuable insights into the practical applications of calculus.

\subsection*{Future Research and Suggestions}
Future work could involve exploring more complex mathematical models and applying these concepts to real-world engineering problems to further bridge the gap between theory and practice.
























\end{document}
