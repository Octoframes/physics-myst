

## Polar Coordinates

See [radial](#polar_animation1_radial) and [theta](#polar_animation1_theta) for animations. See [](#polar_overview) for a static image, and  [trans](#eq:trans) and  [transback](#eq:transback) .


Polar coordinates are a two-dimensional coordinate system in which each point on a plane is determined by a distance from a reference point and an angle from a reference direction.

The reference point (also called the pole) is typically denoted as $O$. The ray from the pole in the reference direction is the positive x-axis, and it's often referred to as the polar axis.

The distance from the pole is called the radial coordinate or radius, and it's often denoted by $r$. The angle from the polar axis is the angular coordinate or the polar angle, typically denoted by $\theta$.

In summary, a point in the plane can be expressed in polar coordinates as $(r, \theta)$, where $r$ is the radial distance and $\theta$ is the polar angle.

To convert from Cartesian coordinates $(x, y)$ to polar coordinates $(r, \theta)$:


\begin{equation} \label{eq:trans}
\begin{bmatrix}r \\ \theta \end{bmatrix} 
= 
\begin{bmatrix}
\sqrt{x^2 + y^2} \\
\text{atan2}(y, x)
\end{bmatrix}
\end{equation}

To convert from polar coordinates $(r, \theta)$ to Cartesian coordinates $(x, y)$:

$$  \label{eq:transback}
\begin{bmatrix}x \\ y \end{bmatrix} 
= r \cdot 
\begin{bmatrix}
\cos(\theta) \\
\sin(\theta)
\end{bmatrix}
$$

**Note:** 
1. The $\sqrt{\text{ }}$ function returns the square root of a number.
2. The $\text{atan2}$ function returns the angle in radians between the positive x-axis and the point given by the coordinates on the two-dimensional plane.
3. The $\cos$ and $\sin$ functions return the cosine and sine of an angle respectively.


:::{figure} #polar_static
:name: polar_overview
:width: 50px
Static cartesian coordinate
:::







::::{note} Some animations
:class: dropdown

:::{figure} #polar_ani1
:name: polar_animation1_radial
:width: 50px
Radial direction
:::


:::{figure} #polar_ani2
:name: polar_animation1_theta
:width: 50px
Theta direction
:::



::::


