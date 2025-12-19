\documentclass[reprint, amsmath,amssymb, aps, prl]{revtex4-2}

\usepackage{graphicx}% Include figure files
\usepackage{dcolumn}% Align table columns on decimal point
\usepackage{bm}% bold math

\begin{document}

\preprint{APS/123-QED}

\title{Collective behavior based on agent-environment interactions}

\author{Gastón Briozzo}
\author{Gustavo J. Sibona}
\affiliation{Facultad de Matemática, Astronomía, Física y Computación (FaMAFyC), Universidad Nacional de Córdoba (UNC), Ciudad Universitaria, (5000) Córdoba, Argentina.\\}
\affiliation{Instituto de Física Enrique Gaviola (IFEG), CONICET, Ciudad Universitaria, (5000) Ćordoba, Argentina.}
\author{Fernando Peruani}
\affiliation{Lab. de Physique Théorique et Modélisation (UMR 8089), CY Cergy Paris Université, 2 avenue A. Chauvin, 95302 Cergy-Pontoise cedex, France\\}

\date{\today}

\maketitle

\section{Supplemental Material}

    This section includes videos showing the evolution of the system from a random initial state to the three states described in the section \textit{Collective Behavior}.
    The tumbling rate used is $\gamma=0.01$ in the video Noise.mp4, $\gamma=0.1$ in the video TravelingWave.mp4 and $\gamma=0.5$ in the video SearchGroups.mp4.
    A time step $dt=0.05$ was used in the simulations. To make the videos, $1$ out of $50$ time steps were recorded and displayed at $20 fps$.
    Animations cover a span of $60000$ time steps.

    The system will start from a initial population $N_0=200$ of disk-shaped agents of radius $r_a=1$, metabolic rate $c=0.005$ and kinetic rate $d_2=0.0005$. 
    Agents have an intake slope $I_s=0.01$ and an intake capacity $I_c = 0.1$. The starvation, reproduction and birth energies are $e_s=0.1$, $e_r=0.9$ and $e_b=0.4$ respectively.
    The environment consist in a squared area of size $L=150$, with periodic boundaries conditions, divided into $m=225$ squared patches of size $L_p=10$, each of them with a food capacity $c_p=1$ and growth rate $r=0.05$. 

    The active speed and the tumbling frequency of the agents have been set at $v_0=2^{-0.5}$ and $\lambda=2^{-9.5}$.

    The initial state of the system is stated as follows
    \begin{equation}
        \begin{split}
            \vec{x}_i(0) &= \left( U_{i,x}(0,L), U_{i,y}(0,L) \right) ~~~~ \forall i \in \left[1, N_0\right], \\
            \theta_i(0)  &= U_{i,\theta}(-\pi, \pi) ~~~~ ~~~~~~~~~~~~~~ \forall i \in \left[1, N_0\right], \\
            e_i(0)  &= U_{i,e}(e_s, e_r) ~~~~~ ~~~~~~~~~~~~~~ \forall i \in \left[1, N_0\right], \\
            f_j(0)  &= U_{j,f}(0, c_p) ~~~~~~ ~~~~~~~~~~~~~~ \forall j \in \left[1, m\right], \\
        \end{split}
    \end{equation}    
 where $U(a,b)$ is a random variable uniformly distributed between values $a$ and $b$.    
\end{document}