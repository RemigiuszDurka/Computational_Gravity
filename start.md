# Computational Gravity 2025

## Course Description

This course is designed to provide students with an in-depth understanding of the use of modern computational tools in the study of gravitational physics, including General Relativity. The course will cover a range of topics, including the use of Mathematica and Cadabra for numerical and symbolic computations, as well as the use of other tools and techniques for studying gravitational models. In addition to lectures, the course will include hands-on laboratory sessions to give students practical experience with the tools and techniques covered in the course.

During the course, we will intelligently **utilize modern computational tools** and **artificial intelligence** to outsource selected aspects of analysis, allowing us to focus on interpreting results and building a deeper understanding of the subject.

Specifically, we will use tools such as: **Python** (sympy, numpy, scipy), **Mathematica**, **Cadabra**, and computational platforms like **Google Colab**, which enable fast and efficient symbolic and numerical calculations. The goal is not only to develop analytical skills but also to gain proficiency in using modern methods that support scientific research.

## Course Goals:

- To provide students with a deep understanding of the use of modern computational tools in the study of gravitational physics.

- To give students practical experience with using Mathematica, Cadabra, and other tools for symbolic and numerical computations.

- To introduce students to a wide range of topics within gravitational physics, including General Relativity.

The laboratory sessions will give students practical experience with the tools and techniques covered in the course, preparing them to use these tools in their own research. The course will also introduce students to a wide range of topics within gravitational physics, providing a solid foundation for further study in the field.

## Course Schedule:

The course will be a total of 30 hours long, split between lectures and laboratory sessions (15h+15h).

## Passing Criteria:

Passing grade will be based on the following criteria:
- Attendance and activity.
- Completion of assignments and presenting outcomes.

There is only grade for the laboratory.

## Requirements for the course:

- Github account
- Colab
- Mathematica
- Cadabra
- AI: ChatGPT, DeepSeek, Qwen, Claude, Gemini, Grok, Kiwi, Copilot, etc.

If you have any **hesitations to use your credentials** to access your colab/AI accounts please:

- consider using your own laptop for the course
- setting additional google account for the course.

# Computational Tools for the Course

## Symbolic and Numerical Computation

In this course, we will use both symbolic and numerical tools to handle complex mathematical structures in General Relativity (GR) and computational gravity. The primary tools will be:

### **Mathematica**
Mathematica is a powerful symbolic and numerical computation software. The following key functions will be used extensively:

- **Simplify / FullSimplify**: To simplify algebraic expressions, particularly tensor calculations in GR.
  $$\text{Simplify}[ \text{expression} ]$$
- **Solve / NSolve**: To find exact and numerical solutions to algebraic equations.
  $$\text{Solve}[ \text{eqn}, x ]$$
- **DSolve**: For solving differential equations analytically and numerically.
  $$\text{DSolve}[ y''[x] + y[x] == 0, y[x], x ]$$
- **NDSolveValue**: For numerical solutions of differential equations.
  $$\text{NDSolveValue}[ y''[x] + y[x] == 0, y, \{x, 0, 10\} ]$$
- **Substitute (ReplaceAll /. )**: To substitute values and simplify expressions dynamically.
  $$\text{expression} /. \{x -> 3, y -> 5\}$$
- **Plot / Plot3D**: Visualization of functions and solutions.
  $$\text{Plot}[\sin(x), \{x, 0, 10\}]$$
and $$\text{Plot3D}[\sin(x) \cos(y), \{x, 0, 10\}, \{y, 0, 10\}]$$

Check:
- [Wolfram Mathematica Documentation](https://reference.wolfram.com/language/) for detailed functions and examples
- [Wolfram Mathematica Tutorials](https://www.wolfram.com/language/fast-introduction-for-programmers/en/) for quick start guides
- [Wolfram Mathematica Stack Exchange](https://mathematica.stackexchange.com/) for community support
- [Wolfram Mathematica Online](https://www.wolframcloud.com/) for cloud-based computation
- [https://community.wolfram.com/groups/-/m/t/2713818](https://community.wolfram.com/groups/-/m/t/2713818) xTensor for GR computations in Mathematica
- [diffgeo.m](https://sites.google.com/view/matthew-headrick/mathematica) for differential geometry in Mathematica
- [https://web.physics.ucsb.edu/~gravitybook/mathematica.html](https://web.physics.ucsb.edu/~gravitybook/mathematica.html) for GR computations in Mathematica
- [https://bhptoolkit.org/KerrGeodesics/](https://bhptoolkit.org/KerrGeodesics/) for Kerr geodesics in Mathematica

### **Cadabra**

Cadabra is a specialized software designed for symbolic manipulation of tensor equations, particularly useful for GR and field theory:

- Tensor manipulations, symmetries, and simplifications.
- Christoffel symbols, Riemann, Ricci tensors computation.
- Automating variation of the Einstein-Hilbert action.

Check out:
- [Cadabra documentation](https://cadabra.science/) for more details
- [https://cadabra.science/help.html](https://cadabra.science/help.html) for tutorials and examples
- [https://cadabra.science/tutorials.html](https://cadabra.science/tutorials.html) for practical guides
- [https://arxiv.org/abs/1912.08839](https://arxiv.org/abs/1912.08839) for a comprehensive guide


### **Python (SymPy, NumPy, SciPy, Matplotlib)**
Python provides a flexible and powerful computational environment with essential libraries for GR:

- [SymPy Documentation](https://docs.sympy.org/latest/index.html)
- [NumPy Documentation](https://numpy.org/doc/stable/)
- [SciPy Documentation](https://docs.scipy.org/doc/scipy/reference/)

- **SymPy** (symbolic computation):
  - Tensor algebra
  - Simplifications
  - Solving differential equations

  ```python
  from sympy import symbols, Eq, solve
  x = symbols('x')
  eq = Eq(x**2 - 4, 0)
  solve(eq, x)
  ```

- **NumPy** (numerical computations, arrays, tensors):
  ```python
  import numpy as np
  A = np.array([[1, 2], [3, 4]])
  np.linalg.inv(A)  # Inverse of matrix
  ```

- **SciPy** (numerical solvers, integration, differential equations):
  ```python
  from scipy.integrate import solve_ivp
  def ode(t, y): return -y
  sol = solve_ivp(ode, [0, 10], [1])
  ```

- **Matplotlib** (visualization):
  ```python
  import matplotlib.pyplot as plt
  plt.plot([0,1,2,3], [0,1,4,9])
  plt.show()
  ```

Check out:

- [https://docs.einsteinpy.org/en/latest/gr_primer.html](https://docs.einsteinpy.org/en/latest/gr_primer.html) dedicated to GR computations in Python
- [https://docs.sympy.org/latest/tutorials/intro-tutorial/intro.html](https://docs.sympy.org/latest/tutorials/intro-tutorial/intro.html)
- [https://docs.scipy.org/doc/scipy/reference/constants.html](https://docs.scipy.org/doc/scipy/reference/constants.html)
---

## Mathematical Frameworks in General Relativity

To understand computational gravity, we require a strong mathematical foundation in:

### **Tensor Calculus**
- Tensor contraction, index raising/lowering
- Christoffel symbols, Riemann and Ricci tensors
- Metric compatibility and curvature computation

### **Differential Equations**
- First and second-order differential equations
- Systems of PDEs describing spacetime evolution
- Numerical integration methods

### **Manifolds and Differential Geometry**
- Differentiable manifolds, charts, and coordinate transformations
- Lie derivatives, Killing vectors
- Curved space metrics, geodesic equations

Link: https://profoundphysics.com/general-relativity-for-dummies/

Books: 

- Sean Carroll, "Spacetime and Geometry: An Introduction to General Relativity"
- Hartle, "Gravity: An Introduction to Einstein's General Relativity"

---

## AI and Modern Computational Assistance

### **Using AI for Research and Computation**
Modern AI tools assist in automating derivations, exploring solutions, and handling large datasets. We will utilize AI-powered assistance to **outsource tasks** and focus on high-level physics:

- **ChatGPT** (OpenAI) – Automates derivations, solves equations, explains concepts.
- **DeepSeek** – Symbolic computation, AI-driven research.
- **Qwen (Alibaba)** – Mathematical reasoning, physics modeling.
- **Claude (Anthropic)** – Scientific insights and tensor algebra assistance.
- **Gemini (Google DeepMind)** – Advanced AI for complex physics and computations.
- **Grok (OpenAI)** – AI-powered assistant.
- **Kiwi (OpenAI)** – yet another AI assistant.
- **Copilot (GitHub)** – AI-powered code completion and suggestions.

These AI tools enable us to speed up calculations, verify derivations, and generate visualizations quickly, allowing us to **focus on the physics rather than tedious computations**.

## Workflow Optimization

To ensure efficiency, the course will integrate:
- **Jupyter Notebooks** in colab for interactive coding (Python, SymPy, NumPy, SciPy)
- **Mathematica Notebooks** for symbolic tensor calculations
- **Latex/Markdown** for documentation and report writing
- **AI-powered assistance** for symbolic derivations and checking calculations

## Course content

1. Modern computational tools.
   
2. Classical gravity: Newtonian gravity, Kepler's laws, two-body problem, three-body problem.

3. Elements of Special Relativity (SR) and General Relativity (GR) description: metric, spacetime interval, Christoffel symbols, Riemann tensor. 

4. Elements of computational Tools: Mathematica, Cadabra, Python, and mathematical frameworks (tensors, differential equations).

5. Geodesics: the paths of test particles in curved spacetime, determined by the geodesic equations. 

6. Einstein's Equations: the fundamental equations of GR that relate the geometry of spacetime (Einstein tensor) to the distribution of energy and momentum (energy-momentum tensor). 

7. Solutions in more details: Schwarzschild, Reissner—Nordstrom, Kerr’a, etc.

8. Cosmological Solutions of Einstein's Equations: an introduction to the Friedmann equations and its significance in describing the evolution of the universe. 

9.  Construction of modified gravity models and the implementation of the variational principle to derive field equations.

10. Other related topics.

## Summary

This course will leverage **Mathematica, Python (SymPy, NumPy, SciPy), Cadabra, and AI-powered tools** to efficiently handle the mathematics of General Relativity and computational gravity. AI tools like **ChatGPT, DeepSeek, Qwen, and others** will help in automating symbolic manipulations, allowing us to focus on the formal expression manipulations, physics of spacetime and numerical simulations. The course will cover a wide range of topics from classical gravity to modern solutions of Einstein's equations, preparing students for advanced research in gravitational physics.

