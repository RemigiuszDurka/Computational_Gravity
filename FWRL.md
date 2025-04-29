# Theoretical and Observational Cosmology 
(notes by dr Remigiusz Durka, 2024)


# Homogeneity and Isotropy in the Universe

The cosmological principle suggests that the universe, on large scales, is both homogeneous and isotropic. This assumption underpins modern cosmological theories and models, including the widely accepted model of the Big Bang.

## Homogeneity and Isotropy: Definitions

1. **Homogeneity**
   - This property implies that the physical conditions (such as density, temperature, and composition) are uniform throughout the universe at any given time. In other words, there is no preferred location in the universe; every place is essentially the same as any other place.
   - Homogeneity means that on a large enough scale, every part of the universe has a similar composition and structure. If the universe is homogeneous, it implies that if you take two large regions of space, each containing many galaxies, they should have a similar number of galaxies, stars, and other forms of matter. 

2. **Isotropy**
   - This property means that the universe looks the same in all directions from any given point. There is no preferred direction in the universe; the cosmos is uniform in all orientations.

Important: While isotropy at every point in space implies homogeneity, the reverse is not necessarily true. A universe can be homogeneous without being isotropic. For example, a universe that expands or contracts differently in different directions is homogeneous but anisotropic.

Example: Consider a large region in space where a magnetic field is uniformly spread out so that the strength of the field is the same everywhere (homogeneous), but the magnetic field lines all go in the same direction (not isotropic).

## Implications of Homogeneity and Isotropy

1. **Time-ordered Sequence of Hypersurfaces**
   - Under these assumptions, the universe can be described as a sequence of three-dimensional space-like hypersurfaces, each representing the state of the universe at a different point in time. These hypersurfaces are homogeneous and isotropic, making them the natural choice for surfaces of constant time.

2. **Symmetry and Geometry**
   - A universe that is both homogeneous and isotropic has the highest possible degree of symmetry, characterized by three independent translations and three rotations in three dimensions. This symmetry significantly constrains the possible geometries of space.
   - There are only three types of homogeneous and isotropic spaces with simple topology:
     - (a) Flat space,
     - (b) A three-dimensional sphere (positive curvature),
     - (c) A three-dimensional hyperbolic space (negative curvature).

## Details of three types of homogeneous and isotropic spaces

1. **Two-dimensional case**
- To better understand these concepts, one can consider two-dimensional analogues of homogeneous and isotropic surfaces, such as the plane (flat space) and the 2-sphere (positive curvature). These can be embedded in three-dimensional Euclidean space using Cartesian coordinates $(x, y, z)$.
- For instance, the embedding of a two-dimensional sphere is described by the equation:
     $$x^2 + y^2 + z^2 = a^2,
     $$
     where $a$ is the radius of the sphere.
- Do $d(...)$ on both sides and express $dz=...$ and $z=...$ using $x,y,r$.
- Plug it to the $ds^2 = dx^2 + dy^2 + dz^2$, and get rid of $z$. 
- Use transition to the polar coordinate system (with r variable): $x=r \cos\phi$, $y=r \sin\phi $, etc.
- The metric suddenly becomes
$$ds^2 = \frac{dr^2}{1 - \left(\frac{r^2}{a^2}\right)} + r^2 d\phi^2.
$$
The limit $a^2 \rightarrow \infty$ corresponds to a (flat) plane. 
- Introducing the rescaled coordinate $r = r'/\sqrt{|a^2|}$, we can recast metric as
$$ds^2 = |a^2|\left( \frac{dr^2}{1 - kr^2} + r^2 d\phi^2 \right),
$$
where $k = +1$ for the sphere ($a^2 > 0$), $k = -1$ for the pseudo-sphere ($a^2 < 0$) and $k = 0$ for the plane (two-dimensional flat space). In curved space, $|a^2|$ characterizes the radius of curvature. In flat space, however, the normalization of $|a^2|$ does not have any physical meaning and this factor can be absorbed by redefinition of the coordinates. 

2. **Three-dimensional case**
The generalization of the above consideration to three dimensions is straightforward:
$$ds^2 = a^2 \left( \frac{dr^2}{1 - kr^2} + r^2(d\theta^2 + \sin^2\theta d\phi^2) \right),$$
After further massaging we obtain also another form used in literature $ds^2 = a^2(d\chi^2 + \phi^2(d\theta^2))$ equal
<p align="center"><img src="https://latex.codecogs.com/svg.latex?\large&space;ds^2%20=%20a^2(d\chi^2%20+%20\phi^2(d\theta^2))%20=%20a^2%20\left\{%20\begin{array}{ll}%20d\chi^2%20+%20\sinh^2\chi%20\,%20d\Omega^2%20&%20\text{for%20}%20k%20=%20-1;%20\\%20d\chi^2%20+%20\chi^2%20\,%20d\Omega^2%20&%20\text{for%20}%20k%20=%200;%20\\%20d\chi^2%20+%20\sin^2\chi%20\,%20d\Omega^2%20&%20\text{for%20}%20k%20=%20+1,%20\end{array}\right." /></p>


# Metrics

## 3 Dimensions: Metrics

1. **Euclidean Metric in Cartesian Coordinates**
   - Definition: The distance in three-dimensional Euclidean space is given by
     $$ds^2 = dx^2 + dy^2 + dz^2.
     $$

2. **Euclidean Metric in Spherical Coordinates (k=0)**
   - Conversion to spherical coordinates $(r, \theta, \phi)$:
     $$ds^2 = dr^2 + r^2(d\theta^2 + \sin^2\theta d\phi^2).
     $$

3. **Metric of a 3D-Sphere (k=1)**
   - In spherical coordinates $(\chi, \theta, \phi)$:
     $$ds^2 = a^2(d\chi^2 + \sin^2\chi(d\theta^2 + \sin^2\theta d\phi^2)),
     $$
     where $a$ is the radius of the 3-sphere.

4. **Metric of a 3D Pseudosphere (k=-1)**
   - For a hyperbolic space:
     $$ds^2 = a^2(d\chi^2 + \sinh^2\chi(d\theta^2 + \sin^2\theta d\phi^2)).
     $$

All cases are realisation of $k=\{0,1,-1\}$
$$ds^2 = a^2 \left( \frac{dr^2}{1 - kr^2} + r^2(d\theta^2 + \sin^2\theta d\phi^2) \right),
$$

## 4 Dimensions: Metrics

1. **Minkowski Metric**

In contrast to the Euclidean metric, Minkowski spacetime incorporates time as a fourth dimension, which is intertwined with the three spatial dimensions. This is fundamental to the special theory of relativity.
   - The interval (distance) in Minkowski spacetime is given by
     $$ds^2 = c^2dt^2 - dx^2 + dy^2 + dz^2,
     $$
     where $c$ is the speed of light in vacuum, and $dt$ represents the time interval.
   - The interval (distance) in Minkowski spacetime in spherical coordinates is given by:
     $$ds^2 = c^2 dt^2 - dr^2 - r^2(d\theta^2 + \sin^2\theta d\phi^2).
     $$
- The negative sign before the time component ($c^2dt^2$) reflects the difference between time and space in relativity and leads to the concept of spacetime interval being invariant under Lorentz transformations (this invariance is crucial for the laws of physics being the same for all observers, regardless of their relative motion).
a
- The Minkowski spacetime metric in 4D allows for the description of events and causal relationships between them, defining light cones and the structure of causality in the universe.

2. **FLRW Metric**
- The Friedmann–Lemaître–Robertson–Walker metric, incorporating scale factor $a(t)$ and curvature $k$, is
  $$ds^2 = dt^2 - a(t)^2 \left(\frac{dr^2}{1 - kr^2} + r^2(d\theta^2 + \sin^2\theta d\phi^2)\right).
  $$

- $a(t)$ is the scale factor, which describes how distances in the universe expand or contract over time.

# General Relativity

At the heart of GR there are two variables: metric $g$ (describing the infinitesimal distance between two points) and connection $\Gamma$ (describing how things change during arallel transport between two infinitesimally distanced points).

Einstein postulates, $\nabla g=0$ and the antisymmetric part of the connection be zero, making the connection a function of the metric $\Gamma(g)$ and expressed by the so-called Christoffel symbols.

## Geodesic Equation

- The geodesic equation describes the path of least action (extremal path) through spacetime:
  $$\frac{d^2 x^\lambda}{d\tau^2} + \Gamma^\lambda_{\mu\nu} \frac{dx^\mu}{d\tau} \frac{dx^\nu}{d\tau} = 0,
  $$
  where $\Gamma^\lambda_{\mu\nu}$ are the Christoffel symbols of the second kind.

## Connection

1. **Definition and Significance**
- In differential geometry, a connection provides a way to compare vectors at different points on a manifold. It is a tool that allows for the transport of vectors along curves in a manifold.
- Mathematically, a connection helps define how much a vector field changes as one moves along a curve within the space, and it is essential for defining the concept of parallel transport.

2. **Application in General Relativity**
- In the context of General Relativity, connections are used to describe how spacetime is curved. They are fundamental in expressing the laws of physics in a form that is independent of the choice of coordinate system.

## Differential Derivative

1. **Covariant Derivative**
- The covariant derivative is a way of specifying a derivative along the curves within a manifold. Unlike ordinary derivatives, the covariant derivative takes into account the curvature of the space $\partial\to \nabla=\partial + \Gamma$.
- It generalizes the notion of a directional derivative from flat spaces to curved spaces. The covariant derivative of a tensor field extends the concept of the directional derivative to fields that can change from point to point in space.
- For a contravariant vector field $X^\lambda$ we have:
$$X^\lambda_{; \mu} \equiv \partial_\mu X^\lambda + \Gamma^\lambda_{\mu \nu} X^\nu$$
- For a covariant vector field $X_\lambda$ we have:
$$X_{\lambda ; \nu} \equiv \partial_\nu X_\lambda - \Gamma^\mu_{\nu \lambda} X_\mu$$
## Christoffel Symbols

1. **Definition and Calculation**

- The Christoffel symbols are mathematical objects that embody the connection coefficients in the framework of Riemannian geometry. They are crucial in defining the Levi-Civita connection, which is a connection in the tangent bundle that is torsion-free and metric-compatible.
- In local coordinates, the Christoffel symbols $\Gamma^\lambda_{\mu \nu}$ are given by the expression:
$${\displaystyle\Gamma^\lambda_{\mu \nu} = \frac{1}{2} g^{\lambda \sigma} (\partial_\mu g_{\nu \sigma}+ \partial_\nu g_{\mu \sigma} - \partial_\sigma g_{\mu \nu})}$$
where $g_{\mu \nu}$ is the metric tensor, and $g^{\mu \nu}$ is its inverse.

2. **Role in Geodesics and Curvature**
- Christoffel symbols are used in the geodesic equation, which describes the paths that particles follow when they are moving without any external forces in a curved spacetime.
- They also appear in the equations defining the Riemann curvature tensor, which measures the intrinsic curvature of a space.

## Christoffel Symbols

For spacetime computations use spliting $(t,i)$, where $i=\{r,\theta,\phi\}$, and scenarios: {tt}, {ti}, {ij}.
- For the FLRW metric (for simplicity k=0):
  $$\Gamma^i_{00} = \Gamma^0_{i0} = \Gamma^0_{00} = 0, \quad \Gamma^i_{jk} = \text{(calculated based on the FLRW metric components)}.
  $$
- Task: Calculate specific Christoffel symbols (FLRW) with students on the blackboard.

## Ricci Tensor
- Definition:
$$R_{\mu\nu}=g^{\alpha \beta} R_{\alpha\mu\beta\nu}
$$
- Expressed through Christoffel symbols:
  $$R_{\mu\nu} = \partial_\lambda \Gamma^\lambda_{\mu\nu} - \partial_\nu \Gamma^\lambda_{\mu\lambda} + \Gamma^\lambda_{\mu\nu}\Gamma^\rho_{\lambda\rho} - \Gamma^\rho_{\mu\lambda}\Gamma^\lambda_{\nu\rho}.
  $$
- Calculate specific components of Einstein tensor $G_{\mu\nu}$ for the FLRW metric.

## Ricci curvature scalar

- Expressed as a contraction
  $$R= g^{\mu\nu} R_{\mu\nu}
  $$
## Einstein Tensor

- Once you have the Ricci tensor, calculate the Einstein tensor:
  $$G_{\mu\nu} = R_{\mu\nu} - \frac{1}{2}g_{\mu\nu}R,
  $$
  where $R$ is the Ricci scalar.

## Energy-Momentum Tensor for Perfect Fluid in Minkowski Space
Matter is incorporated in Einstein’s equations through the (symmetric)  energy–momentum tensor, $T^{\mu\nu}$. In General Relativity the term “matter” is used for anything not the gravitational field. It comes from variating the action $S_{gravity} +S_{matter}$ with respect of metric. Examples: EM action.

- Introduce the energy-momentum tensor for a perfect fluid:
  $$T_{\mu\nu} = (\varepsilon + p)u_\mu u_\nu - pg_{\mu\nu},
  $$
  where $\varepsilon$ is energy density, $p$ is pressure, and $u^\mu$ is the [four-velocity](https://en.wikipedia.org/wiki/Four-velocity).

Remark: The equation of state $p = p(\varepsilon)$ depends on the properties of matter and must
be specified. For example, if the Universe is composed of ultra-relativistic gas, the
equation of state is $p = \varepsilon/3$. In many cosmologically interesting cases $p = w \varepsilon$, where w is constant.

The four-velocity satisfies ${\displaystyle u^{\alpha }u^{\beta }g_{\alpha \beta }=\pm c^{2}}$. In an inertial frame of reference comoving with the fluid, better known as the fluid's proper frame of reference, the four-velocity is ${\displaystyle u^{\alpha }=(1,0,0,0)\,,}$
and the stress–energy tensor is a diagonal matrix 
<p align="center"><img src="https://latex.codecogs.com/svg.latex?\large&space;T_{\mu\nu}=\left(\begin{matrix}\varepsilon&0&0&0\\0&-p\,g_{rr}&0&0\\0&0&-p\,g_{\theta\theta}&0\\0&0&0&-p\,g_{\phi\phi}\end{matrix}\right)" /></p>

with $g_{ij}$ read from FLWR metric.
## Extra task: Divergence of Energy-Momentum Tensor

- Calculate the covariant divergence of $T^{\mu\nu}$ in flat space and then in FLRW space.

## Einstein's Equations

- General form of ten second order differential equations determining variable $g_{\mu\nu}$ defining interval $ds^2 = g_{\mu\nu} dx^\mu dx^\nu.$:
  $$G_{\mu\nu} + \Lambda g_{\mu\nu} = \frac{8\pi G}{c^4} T_{\mu\nu}.$$

Task: Einstein equations -> FLRW metric -> Friedmann equations.

## The Friedmann equations are:

1. The first Friedmann equation:
   $$\left(\frac{\dot{a}}{a}\right)^2 = \frac{8\pi G}{3}\varepsilon - \frac{k}{a^2} + \frac{\Lambda}{3}$$
   
2. The second Friedmann equation:
   $$\frac{\ddot{a}}{a} = -\frac{4\pi G}{3}(\varepsilon+ 3p) + \frac{\Lambda}{3}
   $$
   where:
      - $\varepsilon$ is the energy density of the universe.
   - $k$ is the curvature parameter, which can take values 0, 1, or -1, corresponding to flat, closed, and open universes, respectively.
   - $\Lambda$ is the cosmological constant, representing the energy density of the vacuum of space.
   - $p$ is the pressure of the universe.


## Assignments:
- Derive the Friedman equations from Einstein's equations with the FRW metric.

- Students derive specific components of tensors, Christoffel symbols, and work on up to obtaining the Friedman equations.

