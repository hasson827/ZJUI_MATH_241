# Vector Functions

## Vector Functions and Space Curves

### Vector-Valued Function

In general, a function is a rule that assigns to each element in the domain an element in the range.

A **vector-valued function**, or **vector function**, is simply a function whose domain is a set of real numbers and whose range is a set of vectors.We are most interested in vector functions $\boldsymbol{r}$ whose values are three-dimensional vectors.

This means that for every number $t$ in the domain of $\boldsymbol{r}$ there is a unique vector in $V_3$ denoted by $\boldsymbol{r}(t)$.

If $f(t),g(t)$ and $h(t)$ are the components of the vector $\boldsymbol{r}(t)$, then $f,g,h$ are real-valued functions called the **component functions** of $\boldsymbol{r}$ and we can write
$$
\boldsymbol{r}(t)=\langle f(t),g(t),h(t) \rangle = f(t)\boldsymbol{i} + g(t)\boldsymbol{j} + h(t)\boldsymbol{k}
$$
We use the letter $t$ to denote the independent variable because it representst ime in most applications of vector functions.

### Limits and Continuity

The **limit** of a vector function $\boldsymbol{r}$ is defined by taking the limits of its component functions as follows.

If $\boldsymbol{r}(t)=\langle f(t),g(t),h(t) \rangle$, then
$$
\lim_{t\to a}\boldsymbol{r}(t)=\left\langle \lim_{t\to a}f(t),\lim_{t\to a}g(t),\lim_{t\to a}h(t) \right\rangle
$$
provided the limits of the component functions exist.

A vector function $\boldsymbol{r}$ is **continuous** at $a$ if
$$
\lim_{t\to a}\boldsymbol{r}(t)=\boldsymbol{r}(a)
$$
we see that $\boldsymbol{r}$ is continuous at $a$ if and only if its component functions $f,g,h$ are continuous at $a$.

### Space Curves

There is a close connection between continuous vector functions and space curves.

Suppose that $f,g,h$ are continuous real-valued functions on an interval $I$. Then the set $C$ of all points $(x,y,z)$ in space, where
$$
x=f(t)\quad y=g(t)\quad z=h(t)
$$
and $t$ varies throughout the interval $I$, is called a **space cure**. The equations above are called **parametric equations of $C$** and $t$ is called a **parameter**.

We can think of $C$ as being traced out by a moving particle whose position at time $t$ is $(f(t),g(t),h(t))$. If we now consider the vector function  $\boldsymbol{r}(t)=\langle f(t),g(t),h(t) \rangle$, then $\boldsymbol{r}(t)$ is the position vector the point $P(f(t),g(t),h(t))$ on $C$.

Thus any continuous vector function $\boldsymbol{r}$ defines a space curve $C$ that is traced out by the tip of the moving vector $\boldsymbol{r}(t)$.

## Derivatives and Integrals of Vector Functions

### Derivatives

The derivative $\boldsymbol{r}'$ of a vector function $\boldsymbol{r}$ is defined in much the same way as for real-valued functions:
$$
\frac{d\boldsymbol{r}}{dt}=\boldsymbol{r}'(t)=\lim_{h\to0}\frac{\boldsymbol{r}(t+h)-\boldsymbol{r}(t)}{h}
$$
if this limit exists.

If the points $P$ and $Q$ have position vectors $\boldsymbol{r}(t)$ and $\boldsymbol{r}(t+h)$, then $\vec{PQ}$ represents the vector $\boldsymbol{r}(t+h)-\boldsymbol{r}(t)$, which can therefore be regarded as a secant vector. If $h>0$, the scalar multiple $\left(\frac{1}{h}\right)(\boldsymbol{r}(t+h)-\boldsymbol{r}(t))$ has the same direction as $\boldsymbol{r}(t+h)-\boldsymbol{r}(t)$. As $h\to0$, it appears that this vector approaches a vector that lies on the tangent line. For this reason, the vector $\boldsymbol{r}'(t)$ is called the **tangent vector** to the curve defined by $\boldsymbol{r}$ at the point $P$, provided that $\boldsymbol{r}'(t)$ exists and $\boldsymbol{r}'(t)\ne\boldsymbol{0}$. The **tangent line** to $C$ at $P$ is defined to be the line through $P$ parallel to the tangent vector $\boldsymbol{r}'(t)$.

If $\boldsymbol{r}(t)=\langle f(t),g(t),h(t) \rangle=f(t)\boldsymbol{i}+g(t)\boldsymbol{j}+h(t)\boldsymbol{k}$, where $f,g,h$ are differentiable functions, then
$$
\boldsymbol{r}'(t)=\langle f'(t),g'(t),h'(t) \rangle=f'(t)\boldsymbol{i}+g'(t)\boldsymbol{j}+h'(t)\boldsymbol{k}
$$
A unit vector that has the same direction as the tangent vector is called the **unit tangent vector** $\boldsymbol{T}$ and is defined by
$$
\boldsymbol{T}(t)=\frac{\boldsymbol{r}'(t)}{|\boldsymbol{r}'(t)|}
$$

### Differentiation Rules

Suppose $\boldsymbol{u}$ and $\boldsymbol{v}$ are differentiable vector functions, $c$ is a scalar, and $f$ is a real-valued function. Then
$$
\begin{aligned}
\frac{d}{dt}[ \boldsymbol{u}(t)+\boldsymbol{v}(t)]&=\boldsymbol{u}'(t)+\boldsymbol{v}'(t)
\\[5pt]
\frac{d}{dt}[c\boldsymbol{u}(t)]&=c\boldsymbol{u}'(t)
\\[5pt]
\frac{d}{dt}[f(t)\boldsymbol{u}(t)]&=f'(t)\boldsymbol{u}(t)+f(t)\boldsymbol{u}'(t)
\\[5pt]
\frac{d}{dt}[\boldsymbol{u}(t)\cdot\boldsymbol{v}(t)]&=\boldsymbol{u}'(t)\cdot\boldsymbol{v}(t)+\boldsymbol{u}(t)\cdot\boldsymbol{v}'(t)
\\[5pt]
\frac{d}{dt}[\boldsymbol{u}(t)\times\boldsymbol{v}(t)]&=\boldsymbol{u}'(t)\times\boldsymbol{v}(t)+\boldsymbol{u}(t)\times\boldsymbol{v}'(t)
\\[5pt]
\frac{d}{dt}[\boldsymbol{u}(f(t))]&=f'(t)\boldsymbol{u}'(f(t))
\end{aligned}
$$
**Theorem**: If $|\boldsymbol{r}(t)|=c$ (a constant), then $\boldsymbol{r}'(t)$ is orthogonal to $\boldsymbol{r}(t)$ for all $t$. 

**Proof**: Since
$$
\boldsymbol{r}(t)\cdot\boldsymbol{r}(t)=|\boldsymbol{r}(t)|^2=c^2
$$
and $c^2$ is a constant. Therefore
$$
0=\frac{d}{dt}[\boldsymbol{r}(t)\cdot\boldsymbol{r}(t)]=\boldsymbol{r}'(t)\cdot\boldsymbol{r}(t)+\boldsymbol{r}(t)\cdot\boldsymbol{r}'(t)=2\boldsymbol{r}'(t)\cdot\boldsymbol{r}(t)
$$
Thus $\boldsymbol{r}'(t)\cdot\boldsymbol{r}(t)=0$, which says that $\boldsymbol{r}'(t)$ is orthogonal to $\boldsymbol{r}(t)$.

### Integrals

The definite integral of a continuous vector function $\boldsymbol{r}(t)$ can be defined in much the same way as for real-valued functions except that the integral is a vector. But then we can express the integral of $\boldsymbol{r}$ in terms of the integrals of its component functions $f,g,h$ as follows.
$$
\begin{aligned}
\int_{a}^{b}\boldsymbol{r}(t)dt&=\lim_{n\to\infin}\sum_{i=1}^{n}\boldsymbol{r}(t_i^*)\Delta t 
\\[10pt]
&= \lim_{n\to\infin}\left[ \left(\sum_{i}^{n}f(t_i^*)\Delta t\right)\boldsymbol{i}+\left(\sum_{i}^{n}g(t_i^*)\Delta t\right)\boldsymbol{j}+\left(\sum_{i}^{n}h(t_i^*)\Delta t\right)\boldsymbol{k} \right]
\end{aligned}
$$
So
$$
\int_{a}^{b}\boldsymbol{r}(t)dt=\left( \int_a^bf(t)dt \right)\boldsymbol{i}+\left( \int_a^bg(t)dt \right)\boldsymbol{j}+\left( \int_a^bh(t)dt \right)\boldsymbol{k}
$$
This means that we can evaluate an integral of a vector function by integrating each component function.

We can extend the Fundamental Theorem of Calculus to continuous vector functions as follows:
$$
\int_a^b\boldsymbol{r}(t)dt=\boldsymbol{R}(t)]_a^b=\boldsymbol{R}(b)-\boldsymbol{R}(a)
$$
Where $\boldsymbol{R}$ is an antiderivative of $\boldsymbol{r}$, that is, $\boldsymbol{R}'(t)=\boldsymbol{r}(t)$. We use the notation $\int\boldsymbol{r}(t)dt$ for indefinite integrals (antiderivatives).

## Arc Length and Curvature

### Arc Length

We have defined the length of a plane curve with parametric equations $x=f(t),\;y=g(t),\;a\le t\le b$, as the limit of lengths of inscribed polygons and, for the case where $f'$ and $g'$ are continuous, we arrived at the formula
$$
L=\int_a^b\sqrt{[f'(t)]^2+[g'(t)]^2}dt=\int_a^b\sqrt{\left(\frac{dx}{dt}\right)^2+\left(\frac{dy}{dt}\right)^2}dt
$$
The length of a space curve is defined in exactly the same way.

Suppose that the curve has the vector equation, $\boldsymbol{r}(t)=\langle f(t),g(t),h(t) \rangle,\;a\le t\le b$, or equivalently, the parametric equations $x=f(t),\;y=g(t),\;z=h(t)$, where $f',g',h'$ are continuous. If the curve is traversed exactly once as $t$ increases from $a$ to $b$, then it can be shown that its length is
$$
\begin{aligned}
L=\int_a^b\sqrt{[f'(t)]^2+[g'(t)]^2+[h'(t)]^2}dt=\int_a^b\sqrt{\left(\frac{dx}{dt}\right)^2+\left(\frac{dy}{dt}\right)^2+\left(\frac{dz}{dt}\right)^2}dt
\end{aligned}
$$
Notice that both of the arc length formulas can be put into the more compact form
$$
L=\int_a^b|\boldsymbol{r}'(t)|dt
$$
A single curve $C$ can be represented by more than one vector function. For instance, the twisted cubic
$$
\boldsymbol{r}_1(t)=\langle t,t^2,t^3 \rangle\quad1\le t\le2
$$
could also be represented by the funtion
$$
\boldsymbol{r}_2(u)=\langle e^u,e^{2u},e^{3u} \rangle\quad1\le t \le\ln2
$$
where the connection between the parameters $t$ and $u$ is given by $t=e^u$.

We say that the two formulas above are **parametrizations** of the curve $C$.

### Arc Length Function

Now we suppose that $C$ is a curve given by a vector function
$$
\boldsymbol{r}(t)=f(t)\boldsymbol{i}+g(t)\boldsymbol{j}+h(t)\boldsymbol{k}\qquad a\le t\le b
$$
where $\boldsymbol{r}'$ is continuous and $C$ is traversed exactly once as $t$ increases from $a$ to $b$. We define its **arc length function** $s(t)$ by
$$
s(t)=\int_a^t|\boldsymbol{r}'(u)|du=\int_a^t\sqrt{\left(\frac{dx}{du}\right)^2+\left(\frac{dy}{du}\right)^2+\left(\frac{dz}{du}\right)^2}du
$$
If we differentiate both sides, we obtain
$$
\frac{ds}{dt}=|\boldsymbol{r}'(t)|
$$
It is often useful to **parametrize a curve with respect to arc length** because arc length arises naturally from the shape of the curve and does not depend on a particular coordinate system or a particular parametrization.

If a curve $\boldsymbol{r}(t)$ is already given in terms of a parameter $t$ and $s(t)$ is the arc length function, then we may be able to solve for $t$ as a function of $s$: $t=t(s)$. Then the curve can be reparametrized in terms of $s$ by substituting for $t:\boldsymbol{r}=\boldsymbol{r}(t(s))$. 

### Curvature

A parametrization $\boldsymbol{r}(t)$ is called **smooth** on an interval $I$ if $\boldsymbol{r}'$ is continuous and $\boldsymbol{r}'(t)\ne0$ on $I$.

A curve is called **smooth** if it has a smooth parametrization. A smooth curve has no sharp corners or cusps; when the tangent vector turns, it does so continuously.

If $C$ is a smooth curve defined by the vector function $\boldsymbol{r}$, recall that the unit tangent vector $\boldsymbol{T}(t)$ is given by
$$
\boldsymbol{T}(t)=\frac{\boldsymbol{r}'(t)}{|\boldsymbol{r}'(t)|}
$$
and indicates the direction of the curve. $\boldsymbol{T}(t)$ changes direction very slowly when $C$ is fairly straight, but it changes direction more quickly when $C$ bends or twists more sharply.

The **curvature** of $C$ at a given point is **a measure of how quickly the curve changes direction at that point**. Specifically, we define it to be the magnitude of the rate of change of the unit tangent vector with respect to arc length. (We use arc length so that the curvature will be independent of the parametrization.) Because the unit tangent vector has constant length, only changes in direction contribute to the rate of change of $\boldsymbol{T}$

**Definition**: The **curvature** of a curve is
$$
\kappa = \left| \frac{d\boldsymbol{T}}{ds} \right|
$$
where $\boldsymbol{T}$ is the unit tangent vector.

The curvature is easier to compute if it is expressed in terms of the parameter $t$ instead of $s$, so we use the Chain Rule to write
$$
\frac{d\boldsymbol{T}}{dt} = \frac{d\boldsymbol{T}}{ds}\frac{ds}{dt}\quad\text{and}\quad\kappa=\left|\frac{d\boldsymbol{T}}{ds}\right|=\left| \frac{\frac{d\boldsymbol{T}}{dt}}{\frac{ds}{dt}} \right|
$$
And we have $\frac{ds}{dt}=|\boldsymbol{r}'(t)|$, so
$$
\kappa(t)=\frac{|\boldsymbol{T}'(t)|}{|\boldsymbol{r}'(t)|}
$$
**Theorem**: The curvature of the curve given by the vector function $\boldsymbol{r}$ is
$$
\kappa(t)=\frac{|\boldsymbol{r}'(t)\times\boldsymbol{r}''(t)|}{|\boldsymbol{r}'(t)|^3}
$$
**Proof**: Let's define $v(t)=|\boldsymbol{r}'(t)|$, it is a scalar function. Then according to the definition of $\boldsymbol{T}(t)=\frac{\boldsymbol{r}'(t)}{|\boldsymbol{r}'(t)|}=\frac{\boldsymbol{r}'(t)}{v(t)}$, We can compute the derivative of $\boldsymbol{T}'(t)$
$$
\boldsymbol{T}'(t)=\frac{\boldsymbol{r}''(t)v(t)-\boldsymbol{r}'(t)v'(t)}{v(t)^2}
$$
Then the definition of $\kappa(t)=\frac{|\boldsymbol{T}'(t)|}{|\boldsymbol{r}'(t)|}$ gives us
$$
\kappa(t)=\frac{|\boldsymbol{T}'(t)|}{v(t)}
$$
Then we can compute the cross product  $\boldsymbol{r}'(t)\times\boldsymbol{r}''(t)$, we get
$$
\begin{aligned}
\boldsymbol{r}'(t)\times\boldsymbol{r}''(t)&=(v(t)\boldsymbol{T}(t))\times(v(t)\boldsymbol{T}(t))'
\\[5pt]
&=(v(t)\boldsymbol{T}(t))\times(v'(t)\boldsymbol{T}(t)+v(t)\boldsymbol{T}'(t))
\\[5pt]
&=v(t)v'(t)(\boldsymbol{T}(t)\times\boldsymbol{T}(t))+v(t)^2(\boldsymbol{T}(t)\times\boldsymbol{T}'(t))
\\[5pt]
&=v(t)^2(\boldsymbol{T}(t)\times\boldsymbol{T}'(t))
\end{aligned}
$$
Because $\boldsymbol{T}(t)$ is always a unit vector, we have $|\boldsymbol{T}(t)\times\boldsymbol{T}'(t)|=|\boldsymbol{T}(t)||\boldsymbol{T}'(t)|\sin\theta=|\boldsymbol{T}'(t)|$. Therefore, we have
$$
|\boldsymbol{r}'(t)\times\boldsymbol{r}''(t)|=v(t)^2|\boldsymbol{T}'(t)|=v(t)^3\kappa(t)
$$
It's proof is done.

For the special case of a plane curve with equation $y=f(x)$, we choose $x$ as the parameter and write $\boldsymbol{r}(x)=x\boldsymbol{i}+f(x)\boldsymbol{j}$. Then $\boldsymbol{r}'(x)=\boldsymbol{i}+f'(x)\boldsymbol{j}$ and $\boldsymbol{r}''(x)=f''(x)\boldsymbol{j}$. Since $\boldsymbol{i}\times\boldsymbol{j}=\boldsymbol{k}$ and $\boldsymbol{j}\times\boldsymbol{j}=\boldsymbol{0}$, it follows that $\boldsymbol{r}'(x)\times\boldsymbol{r}''(x)=f''(x)\boldsymbol{k}$. We also have $|\boldsymbol{r}'(x)|=\sqrt{1+[f'(x)]^2}$ and so we have
$$
\kappa(x)=\frac{|f''(x)|}{\left[ 1+(f'(x))^2 \right]^{\frac{3}{2}}}
$$

### Normal and Binormal Vectors

At a given point on a smooth space curve $\boldsymbol{r}(t)$, there are many vectors that are orthogonal to the unit tangent vector $\boldsymbol{T}(t)$. We single out one by observing that, because $|\boldsymbol{T}(t)|=1$ for all $t$, we have $\boldsymbol{T}(t)\cdot\boldsymbol{T}'(t)=0$, so $\boldsymbol{T}'(t)$ is orthogonal to $\boldsymbol{T}(t)$. Note that $\boldsymbol{T}'(t)$ is itself not a unit vector.

But at any point where $\kappa\ne0$ we can define the **principal unit normal vector $\boldsymbol{N}(t)$** (or simply **unit normal**) as
$$
\boldsymbol{N}(t)=\frac{\boldsymbol{T}'(t)}{|\boldsymbol{T}'(t)|}
$$
The vector $\boldsymbol{B}(t)=\boldsymbol{T}(t)\times\boldsymbol{N}(t)$ is called the **binormal vector**. It is perpendicular to both $\boldsymbol{T}$ and $\boldsymbol{N}$ and is also a unit vector.

The plane determined by the normal and binormalvectors  $\boldsymbol{N}$ and $\boldsymbol{B}$ at a point $P$ on a curve $C$ is called the **normal plane** of $C$ at $P$. It **consists of all lines that are orthogonal** to the tangent vector $\boldsymbol{T}$. 

The plane determined by the vectors $\boldsymbol{T}$ and $\boldsymbol{N}$ is called the **osculating plane** of $C$ at $P$. It is the plane that comes closest to containing the part of the curve near $P$. (For a plane curve, the osculating plane is simply the plane that contains the curve.)

The **circle of curvature**, or the **osculating circle**, of $C$ at $P$ is the circle in the osculating plane that passes through $P$ with radius $\frac{1}{\kappa}$ and center a distance $\frac{1}{\kappa}$ from $P$ along the vector $\boldsymbol{N}$. The center of the circle is called the **center of curvature** of $C$ at $P$.

### Torsion

Curvature $\kappa=\frac{|d\boldsymbol{T}|}{ds}$ at a point $P$ on a curve $C$ indicates how tightly the curve "bends". Since $\boldsymbol{T}$ is a normal vector for the normal plane, $\frac{d\boldsymbol{T}}{ds}$ tells us how the normal plane changes as $P$ moves along $C$.

Since $\boldsymbol{B}$ is normal to the osculating plane, $\frac{d\boldsymbol{B}}{ds}$ gives us information about how the osculating plane changes as $P$ moves along $C$.

Thus there is a scalar $\tau$ such that
$$
\frac{d\boldsymbol{B}}{ds}=-\tau\boldsymbol{N}
$$
The number $\tau$ is called the torsion of $C$ at $P$. It we take the dot product with $\boldsymbol{N}$ of each side and note that $\boldsymbol{N}\cdot\boldsymbol{N}=1$, we get the following definition:

The **torsion** of a curve is 
$$
\tau = -\frac{d\boldsymbol{B}}{ds}\cdot\boldsymbol{N}
$$
From the definition we have
$$
\tau(t)=-\frac{\boldsymbol{B}'(t)\cdot\boldsymbol{N}(t)}{|\boldsymbol{r}'(t)|}
$$

### Velocity, Speed, and Acceleration

Suppose a particle moves through space so that its position vector at time $t$ is $\boldsymbol{r}(t)$, for small values of $h$, the vector
$$
\frac{\boldsymbol{r}(t+h)-\boldsymbol{r}(t)}{h}
$$
approximates the direction of the particle moving along the curve $\boldsymbol{r}(t)$. Its magnitude measures the size of the displacement vector per unit time.

The vector gives the average velocity over a time interval of length $h$ and its limit is the **velocity vector** $\boldsymbol{v}(t)$ at time $t$:
$$
\boldsymbol{v}(t)=\lim_{h\to0}\frac{\boldsymbol{r}(t+h)-\boldsymbol{r}(t)}{h}=\boldsymbol{r}'(t)
$$
Thus the velocity vector is also the tangent vector and points in the direction of the tangent line. The **speed** of the particle at time $t$ is the magnitude of the velocity vector, that is, $|\boldsymbol{v}(t)|$.

As in the case of one-dimensional motion, the **acceleration** of the particle is defined as the derivative of the velocity:
$$
\boldsymbol{a}(t)=\boldsymbol{v}'(t)=\boldsymbol{r}''(t)
$$
In general, vector integrals allow us to recover velocity when acceleration is known and position when velocity is known:
$$
\boldsymbol{v}(t)=\boldsymbol{v}(t_0)+\int_{t_0}^{t}\boldsymbol{a}(u)du
\\[5pt]
\boldsymbol{r}(t)=\boldsymbol{r}(t_0)+\int_{t_0}^{t}\boldsymbol{v}(u)du
$$
If the force taht acts on a particle is known, then the acceleration can be found from **Newton's second law of Motion**. The vector version of this law states that if, at any time $t$, a force $\boldsymbol{F}(t)$ acts on an object of mass $m$ producint an acceleration $\boldsymbol{a}(t)$, then
$$
\boldsymbol{F}(t)=m\boldsymbol{a}(t)
$$

### Projectile Motion (抛物运动)

A projectile is fired with angle of elevation $\alpha$ and initial velocity $\boldsymbol{v}_0$. Assuming that air resistance is negligible and the only external force is due to gravity, find theposition function $\boldsymbol{r}(t)$ of the projectile. What value of $\alpha$ maximizes the range (the horizontal distance traveled)?

We set up the axes so that the projectile starts at the origin. Since the force due to gravity acts downward, we have
$$
\boldsymbol{F}=m\boldsymbol{a}=-mg\boldsymbol{j}
$$
Where $|g|=\boldsymbol{a}\approx9.8\mathrm{m/s}^2$. Thus
$$
\boldsymbol{a}=-g\boldsymbol{j}
$$
Since $\boldsymbol{v}'(t)=\boldsymbol{a}$, we have
$$
\boldsymbol{v}(t)=-gt\boldsymbol{j}+\boldsymbol{C}
$$
where $\boldsymbol{C}=\boldsymbol{v}(0)=\boldsymbol{v}_0$. Therefore
$$
\boldsymbol{r}'(t)=\boldsymbol{v}(t)=-gt\boldsymbol{j}+\boldsymbol{v}_0
$$
Integrating again, we obtain
$$
\boldsymbol{r}(t)=-\frac{1}{2}gt^2\boldsymbol{j}+t\boldsymbol{v}_0+\boldsymbol{D}
$$
But $\boldsymbol{D}=\boldsymbol{r}(0)=\boldsymbol{0}$, so the position vector of the projectile is given by
$$
\boldsymbol{r}(t)=-\frac{1}{2}gt^2\boldsymbol{j}+t\boldsymbol{v}_0
$$
The horizontal distance $d$ is the value of $x$ when $y=0$. Setting $y=0$, we obtain $t=0$ or $t=\frac{2v_0\sin\alpha}{g}$. This second value of $t$ then gives
$$
\begin{aligned}
d=x&=(v_0\cos\alpha)\frac{2v_0\sin\alpha}{g}
\\[5pt]
&=\frac{v_0^2(2\sin\alpha\cos\alpha)}{g}
\\[5pt]
&=\frac{v_0^2\sin2\alpha}{g}
\end{aligned}
$$
Clearly, $d$ has its maximum value when $\sin2\alpha=1$, that is, $\alpha=45\degree$.

### Tangential and Normal Components of Acceleration

When we study the motion of a particle, it is often useful to resolve the acceleration into two components, one in the direction of the tangent and the other in the direction of the normal.

If we write $v=|\boldsymbol{v}|$ for the speed of the particle, then
$$
\boldsymbol{T}(t)=\frac{\boldsymbol{r}'(t)}{|\boldsymbol{r}'(t)|}=\frac{\boldsymbol{v}(t)}{|\boldsymbol{v}(t)|}=\frac{\boldsymbol{v}}{v}\quad\text{and}\quad\boldsymbol{v}=v\boldsymbol{T}
$$
If we differentiate both sides of this equation with respect to $t$, we get
$$
\boldsymbol{a}=\boldsymbol{v}'=v'\boldsymbol{T}+v\boldsymbol{T}'
$$
If we use the expression for the curvature, then we have
$$
\kappa=\frac{|\boldsymbol{T}'|}{|\boldsymbol{r}'|}=\frac{|\boldsymbol{T}'|}{v}\quad\Longrightarrow\quad|\boldsymbol{T}'|=\kappa v
$$
The unit normal vector was defined in the preceding section as $\boldsymbol{N}=\frac{\boldsymbol{T}'}{|\boldsymbol{T}'|}$, so
$$
\boldsymbol{T}'=|\boldsymbol{T}'|\boldsymbol{N}=\kappa v\boldsymbol{N}
$$
and the equation above becomes
$$
\boldsymbol{a}=v'\boldsymbol{T}+\kappa v^2\boldsymbol{N}
$$
Writing $a_T$ and $a_N$ for the tangential and normal components of acceleration, we have
$$
\boldsymbol{a}=a_T\boldsymbol{T}+a_N\boldsymbol{N}
$$
where
$$
a_t=v'\qquad a_N=\kappa v^2
$$
The first thing to notice is that the binormalvector $\boldsymbol{B}$ is absent. No matter how an object moves through space, its acceleration always lies in the plane of $\boldsymbol{T}$ and $\boldsymbol{N}$ (the osculating plane). (Recall that $\boldsymbol{T}$ gives the direction of motion and $\boldsymbol{N}$ points in the direction the curve is turning.) Next we notice that the tangential component of acceleration is $\boldsymbol{v}'$, the rate of change of speed, and the normal component of acceleration is $\kappa v^2$. This makes sense if we think of a passenger in a car: a sharp turn in a road means a large value of the curvature $\kappa$ so the component of the acceleration perpendicular to the motion is large and the passenger is thrown against a car door. High speed around the turn has the same effect, in fact, if you double your speed, $a_N$ increased by a factor of 4. Although we have expressions for the tangential and normal components of acceleration, it's desirable to have expressions that dependonly on $\boldsymbol{r},\boldsymbol{r}'$, and $\boldsymbol{r}''$.

To this end we take the dot product of $\boldsymbol{v}=v\boldsymbol{T}$ with $\boldsymbol{a}$.
$$
\begin{aligned}
\boldsymbol{v}\cdot\boldsymbol{a}&=v\boldsymbol{T}\cdot(v'\boldsymbol{T}+\kappa v^2\boldsymbol{N})
\\[5pt]
&=vv'\boldsymbol{T}\cdot\boldsymbol{T}+\kappa v^3\boldsymbol{T}\cdot\boldsymbol{N}
\\[5pt]
&=vv'
\end{aligned}
$$
Therefore
$$
a_T=v'=\frac{\boldsymbol{v}\cdot\boldsymbol{a}}{v}=\frac{\boldsymbol{r}'(t)\cdot\boldsymbol{r}''(t)}{|\boldsymbol{r}'(t)|}
$$
Using the formula for curvature, we have
$$
a_N=\kappa v^2=\frac{|\boldsymbol{r}'(t)\times\boldsymbol{r}''(t)|}{|\boldsymbol{r}'(t)|^3}|\boldsymbol{r}'(t)|^2=\frac{|\boldsymbol{r}'(t)\times\boldsymbol{r}''(t)|}{|\boldsymbol{r}'(t)|}
$$

### Kepler's Laws of Planetary Motion

**Kepler's Laws**

1. A planet revolves around the sun in an elliptical orbit with the sun at one focus.
2. The line joining the sun to a planet sweeps out equal areas in equal times.
3. The square of the period of revolution of a planet is proportional to the cube of the length of the major axis of its orbit.

Since the gravitational force of the sun on a planet is so much larger than the forces exerted by other celestial bodies, we can safely ignore all bodies in the universe except the sun and one planet revolving about it.
We use a coordinate system with the sun at the origin and we let $\boldsymbol{r}=\boldsymbol{r}(t)$ be the position vector of the planet. (Equally well, $\boldsymbol{r}$ could be the position vector of the moon or a satellite moving around the earth or a comet moving around a star.)

The velocity vector is $\boldsymbol{v}=\boldsymbol{r}'$ and the acceleration vector is $\boldsymbol{a}=\boldsymbol{r}''$. We use the following laws of Newton:
$$
\begin{aligned}
\boldsymbol{F}&=m\boldsymbol{a}
\\[5pt]
F&=-\frac{GMm}{r^3}\boldsymbol{r}=-\frac{GMm}{r^2}\boldsymbol{u}
\end{aligned}
$$
where $\boldsymbol{F}$ is the gravitational force on the planet, $m$ and $M$ are the masses of the planet and the sun, $G$ is the gravitational constant, $r=|\boldsymbol{r}|$, and $\boldsymbol{u}=\frac{\boldsymbol{r}}{r}$ is the unit vector in the direction of $\boldsymbol{r}$.

We first show that the planet moves in one plane. By equating the expressions for $\boldsymbol{F}$ in Newton's two laws, we find that
$$
\boldsymbol{a}=-\frac{GM}{r^3}\boldsymbol{r}
$$
and so $\boldsymbol{a}$ ia parallel to $\boldsymbol{r}$. It follows that $\boldsymbol{r}\times\boldsymbol{a}=\boldsymbol{0}$.
$$
\begin{aligned}
\frac{d}{dt}(\boldsymbol{r}\times\boldsymbol{v})&=\boldsymbol{r}'\times\boldsymbol{v}+\boldsymbol{r}\times\boldsymbol{v}'
\\
&=\boldsymbol{v}\times\boldsymbol{v}+\boldsymbol{r}\times\boldsymbol{a}
\\[5pt]
&=\boldsymbol{0}+\boldsymbol{0}
\\[5pt]
&=\boldsymbol{0}
\end{aligned}
$$
Therefore
$$
\boldsymbol{r}\times\boldsymbol{v}=\boldsymbol{h}
$$
where $\boldsymbol{h}$ is a constant vector. (We may assume that $\boldsymbol{h}\ne\boldsymbol{0}$; that is, $\boldsymbol{r}$ and $\boldsymbol{v}$ are not parallel)

This means that the vector $\boldsymbol{r}=\boldsymbol{r}(t)$ is perpendicular to $\boldsymbol{h}$ for all values of $t$, so the planet always lies in the plane throught the origin perpendicular to $\boldsymbol{h}$. Thus the orbit of the planet is a plane curve.

To prove **Kepler's First Law** we rewrite the vector $\boldsymbol{h}$ as follows:
$$
\begin{aligned}
\boldsymbol{h}&=\boldsymbol{r}\times\boldsymbol{v}=\boldsymbol{r}\times\boldsymbol{r}'=r\boldsymbol{u}\times(r\boldsymbol{u})'
\\[5pt]
&=r\boldsymbol{u}\times(r\boldsymbol{u}'+r'\boldsymbol{u})=r^2(\boldsymbol{u}\times\boldsymbol{u}')+rr'(\boldsymbol{u}\times\boldsymbol{u})
\\[5pt]
&=r^2(\boldsymbol{u}\times\boldsymbol{u}')
\end{aligned}
$$
Then
$$
\begin{aligned}
\boldsymbol{a}\times\boldsymbol{h}&=\frac{-GM}{r^2}\boldsymbol{u}\times[r^2(\boldsymbol{u}\times\boldsymbol{u}')]=-GM\boldsymbol{u}\times(\boldsymbol{u}\times\boldsymbol{u}')
\\[5pt]
&=-GM[(\boldsymbol{u}\cdot\boldsymbol{u}')\boldsymbol{u}-(\boldsymbol{u}\cdot\boldsymbol{u})\boldsymbol{u}']
\end{aligned}
$$
But $\boldsymbol{u}\cdot\boldsymbol{u}=|\boldsymbol{u}|^2=1$ and since $|\boldsymbol{u}(t)|=1$, it follows that $\boldsymbol{u}\cdot\boldsymbol{u}'=0$. Therefore
$$
\boldsymbol{a}\times\boldsymbol{h}=-GM\boldsymbol{u}'
$$
and so
$$
\begin{aligned}
(\boldsymbol{v}\times\boldsymbol{h})'&=\boldsymbol{v}'\times\boldsymbol{h}+\boldsymbol{v}\times\boldsymbol{h}'
\\[5pt]
&=\boldsymbol{a}\times\boldsymbol{h}
\\[5pt]
&=GM\boldsymbol{u}'
\end{aligned}
$$
Integrating both sides of this equation, we get
$$
\boldsymbol{v}\times\boldsymbol{h}=GM\boldsymbol{u}+\boldsymbol{c}
$$
where $\boldsymbol{c}$ is a constant vector.

At this point it is convenient to choose the coordinate axes so that the standard basis vector $\boldsymbol{k}$ points in the direction of the vector $\boldsymbol{h}$. Then the planet moves in the xy-plane. Since both $\boldsymbol{v}\times\boldsymbol{h}$ and $\boldsymbol{u}$ are perpendicular to $\boldsymbol{h}$, the above equation shows that $\boldsymbol{c}$ lies in the xy-plane.

If $\theta$ is the angle between $\boldsymbol{c}$ and $\boldsymbol{r}$, then $(r,\theta)$ are polar coordinates of the planet. we have
$$
\begin{aligned}
\boldsymbol{r}\cdot(\boldsymbol{v}\times\boldsymbol{h})&=\boldsymbol{r}\cdot(GM\boldsymbol{u}+c)=GM\boldsymbol{r}\cdot\boldsymbol{u}+\boldsymbol{r}\cdot\boldsymbol{c}
\\[5pt]
&=GMr\boldsymbol{u}\cdot\boldsymbol{u}+|\boldsymbol{r}||\boldsymbol{c}|\cos\theta
\\[5pt]
&=GM\boldsymbol{r}+rc\cos\theta
\end{aligned}
$$
where $c=|\boldsymbol{c}|$. Then
$$
r=\frac{\boldsymbol{r}\cdot(\boldsymbol{v}\times\boldsymbol{h})}{GM+c\cos\theta}=\frac{1}{GM}\frac{\boldsymbol{r}\cdot(\boldsymbol{v}\times\boldsymbol{h})}{1+e\cos\theta}
$$
where $e=\frac{c}{GM}$. But
$$
\boldsymbol{r}\cdot(\boldsymbol{v}\times\boldsymbol{h})=(\boldsymbol{r}\times\boldsymbol{v})\cdot\boldsymbol{h}=\boldsymbol{h}\times\boldsymbol{h}=h^2
$$
where $h=|\boldsymbol{h}|$. So
$$
r=\frac{\frac{h^2}{GM}}{1+e\cos\theta}=\frac{\frac{eh^2}{c}}{1+e\cos\theta}
$$
Writing $d=\frac{h^2}{c}$, we obtain the equation
$$
r=\frac{ed}{1+e\cos\theta}
$$
we see that the equation is the polar equation of a conic section with focus at the origin and eccentricity $e$. We know that the orbit of a planet is a closed curve and so the conic must be an ellipse.