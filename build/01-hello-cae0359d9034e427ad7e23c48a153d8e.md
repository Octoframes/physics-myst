

## Polar Coordinates

In polar coordinates, points in a plane are defined by radial distance $r$ and angular coordinate $\theta$  ([](#polar_overview)). The [radial direction](#polar_animation1_radial) measures the point's distance from the origin, while the [angular direction](#polar_animation1_theta) corresponds to the counterclockwise angle from the positive x-axis. These two dimensions together specify any point in the plane.

When transitioning from Cartesian coordinates ($x$, $y$) to polar coordinates ($r$, $\theta$), we calculate the radial distance and angle using equation [](#eq:trans). Conversely, when converting from polar back to Cartesian coordinates, we use equation [](#eq:transback).







:::{figure} #polar_static
:name: polar_overview
:width: 50px
Polar coordinate system
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
Angular direction
:::

::::


::::{note} Formulas
:class: dropdown

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

::::


