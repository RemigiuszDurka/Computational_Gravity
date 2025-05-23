# Problems in Computational Gravity

Each problem should have a short markdown code note explaining the setup/theory/goal. The problems should be solved using computational tools like Mathematica, Python, Cadabra, and Geogebra (whatever works!)

1. **Modern computational tools - Preliminary**

    a) Set up: Github account, Colab, Mathematica (wolframcoud/Mathematica 11), and later Geogebra and Cadabra. 
 
    b) Get access to many AI: ChatGPT, DeepSeek, Qwen, Claude, Gemini, Grok, etc. (free access require login, limited number of queries per day can be avoided by using different AI).

2. **Classical gravity**

    a) Consider the free fall problem of two point masses, 1kg each, one meter apart, starting from rest. Find a solution of the problem and time of the collision in hours. Plot x(t) function.

    b) Visualize potential and field lines or vectors for: (a) point mass, (b) two-point mass system, (c) three-point mass system.

    c) Visualize the 3-body problem, give some starting conditions, and various masses, and plot various trajectories (animation example can be found in provided [colab file](https://colab.research.google.com/drive/15PMeEg_V21tQgLgsNld_1Z0_OaPKLCIn?usp=sharing)).

    d) Visualize Hohmann transfer between Earth and Mars (animation example can be found in provided [colab file](https://colab.research.google.com/drive/15PMeEg_V21tQgLgsNld_1Z0_OaPKLCIn?usp=sharing)). Workflow: ask for plot, with code giving plot ask for video animation in colab, with code generating video aks for animated gif in colab)

3. **Basics of SR and GR**

    a) for a given metric be able to compute the inverse metric, Christoffel symbols, Riemann and Ricci tensors, curvature scala and the Einstein tensor components.

    b) incorporate solution scenarios: flat case, with M, with Q, with rotation Kerr parameter $a=J/M$, and compute all quantities listed above.

    c) include cosmological constant $\Lambda$ to Schwarschild case, and Reissner-Nordstrom case. Update Einstein equation to the $+ \Lambda g_{\mu \nu}$ term.
   
    d) Use in computations pure dS spacetime $\Lambda > 0, M=0$.

    d) compare your results with [Catalogue of Spacetimes](https://www2.mpia-hd.mpg.de/homes/tmueller/pages/rela_additional.php) to make sure the results are correct.

    e) Do similar computations for Alcubierre solution [arXiv:gr-qc/0009013](https://arxiv.org/abs/gr-qc/0009013), and Rindler solution.

5. **Parallel transport** 

    Consider a 2D sphere embedded in 3D Euclidean space. For induced metric on the sphere, compute the Christoffel symbols, Riemann tensor, and curvature scalar. Consider parallel transport and compute the geodesic equation. Try to visualize the parallel transport on the sphere.

6. **Geodesic Equation** 

    Write down (as a markdown note) formally the geodesic equations for a Schwarzschild metric. List interesting initial conditions for the Schwarzschild metric and plot the geodesic curves around the Schwarzschild black hole.

---

6. **Implementing the derivation of Reissner-Nordstrom solution**

    Try to computationally repeat derivations given in [link 1](https://www.researchgate.net/publication/336304500_Reissner-Nordstrom_metric) and [link 2](https://www.diva-portal.org/smash/get/diva2:912393/FULLTEXT01.pdf). Try to repeat it for a solution with the cosmological constant. [Extremly hard (publication level: Try to repeat it for a uniform constant electric/magnetic field :)]

7. **Friedmann Equations**

    Derive the Friedmann equations directly from Einstein's field equations for a homogeneous and isotropic universe (use starting general metric ansatz, and define in python energy-momentum tensor). Discuss/visualize the possible solutions $a(t)$ (radiation, dust, cosmological constant, and mixed) and their implications for the evolution of the universe. Discuss the energy density, pressure, and equation of state for each component. 

8. **Variational Principle** 

    Show in python how two Firedmann equations come from the variation principle. Hint: use N(t) and a(t) to produe value of g, R and Einstein-Hilbert action. Write a markdown note with details of variation of the EM in flat Minkowski space. Implement in pyhton FLRW Gravity coupled to the scalar field. 

---

9. **Lagrangian constructing**

    Compute the curvature scalar, Kretschmann scalar (link: [https://arxiv.org/abs/astro-ph/9912320](https://arxiv.org/abs/astro-ph/9912320)), Euler (Gauss-Bonnet) term, and Pontryagin term separately for the Schwarzschild metric, Reissner-Nordstrom metric, and Kerr metric. Compare the values of the [Kretschmann scalar](https://medium.com/@Merrysci/why-kretschmann-scalar-is-important-in-general-relativity-05e58576768e) for these metrics and discuss its physical significance. Try to visualize the curvature of spacetime using the Kretschmann scalar. For the Schwarzschild case use various coordinate systems.
   
10. **Propose some interesting GR problem** and solve it.

## Additional links:

- [Colab BRUDNOPIS Computational Gravity](https://colab.research.google.com/drive/15PMeEg_V21tQgLgsNld_1Z0_OaPKLCIn?usp=sharing)
