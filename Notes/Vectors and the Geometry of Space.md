# Vectors and the Geometry of Space

## Three-Dimensional Coordinate Systems

### 3D Space

In order to represent points in space, we first choose a fixed point $O$ (the origin) and three directed lines through $O$ that are perpendicular to each other, called the **coordinate aces** and labeled the $x$-axis, $y$-axis, and $z$-axis.

The direction of the $z$-axis is determined by the **right-hand rule** as illustrated in the figure:

<img src="/Users/hasson/Library/CloudStorage/OneDrive-InternationalCampus,ZhejiangUniversity/2025_FA_Semester/MATH 241/Notes/assets/image-20250916105919824.png" alt="image-20250916105919824" style="zoom:40%;" />

If you curl the fingers of your right hand around the $z$-axis in the direction of a $90\degree$ counterclockwise rotation from the positive $x$-axis to the positive $y$-axis, then your thumb points in the positive direction of the $z$-axis.

The three coordinate axes determined the three coordinate planes illustrated in the figure.

<img src="/Users/hasson/Library/CloudStorage/OneDrive-InternationalCampus,ZhejiangUniversity/2025_FA_Semester/MATH 241/Notes/assets/image-20250916110748202.png" alt="image-20250916110748202" style="zoom:40%;" />

These three coordinate planes divide space into 8 parts, called **octants**(卦限八分区). The **first octant**, in the foreground, is determined by the positive axes.

Thus, to locate the point $(a,b,c)$, we can start at the origin $O$ and move $a$ units along the $x$-axis, then $b$ units parallel to the $y$-axis, and then $c$ units parallel to the $z$-axis. The point $P(a,b,c)$ determins a rectangular box. If we drop a perpendicular from $P$ to the $xy$-plane, we get a point $Q$ with coordinates $(a,b,0)$ called the **projection** of $P$ onto the $xy$-plane. Similarly, $R(0,b,c)$ and $S(a,0,c)$ are the projections of $P$ onto the $yz$-plane and $xz$-plane, respectively.

<img src="/Users/hasson/Library/CloudStorage/OneDrive-InternationalCampus,ZhejiangUniversity/2025_FA_Semester/MATH 241/Notes/assets/image-20250916111429349.png" alt="image-20250916111429349" style="zoom:40%;" />

The Cartesian product $\R\times\R\times\R = \{(x,y,z)|x,y,z\in\R\}$ is the set of all ordered triples of real numbers and is denoted by $\R^3$.

We have given a one-to-one correspondence between points $P$ in space and an ordered triples $(a,b,c)$ in $\R^3$. It is called a **three-dimensional rectangular coordinate system**. Notice that, in terms of coordinates, the first octant can be described as the set of points whose coordinates are all positive.

### Surfaces and Solids

In two-dimensional analytic geometry, the graph of an equation involving $x$ and $y$ is a curve in $\R^2$. In three-dimensional analytic geometry, an equation in $x,y,z$ represents a surface in $\R^3$

In general, if $k$ is a constant, then $x=k$ represents a plane parallel to the $yz$-plane, $y=k$ is a plane parallel to the $xz$-plane, and $z=k$ is a plane parallel tothe $xy$-plane.

### Distance and Spheres

**Distance Formula in Three Dimensions**: The distance $|P_1P_2|$ between the points $P_1(x_1,y_1,z_1)$ and $P_2(x_2,y_2,z_2)$ is 
$$
\begin{aligned}
|P_1P_2| &= \sqrt{ (x_2-x_1)^2+(y_2-y_1)^2+(z_2-z_1)^2 }
\\[10pt]
&= \sqrt{(P_1-P_2)^T(P_1-P_2)}
\end{aligned}
$$
**Equation of a Sphere**: An equation of a sphere with center $C(h,k,l)$ and radius $r$ is 
$$
(x-h)^2+(y-k)^2+(z-l)^2 = r^2
$$
In particular, if the center is the origin $O$, then an equation of the sphere is 
$$
x^2+y^2+z^2=r^2
$$

## Vectors

The term **vector** is used in mathematics to indicate a quantity that has both magnitude and direction.

### Geometric Description of Vectors

A vector is often represented by an arrow or a directed line segment. The length of the arrow represents the magnitude of the vector and the arrow points in the direction of the vector. We denote a vector by printing a letter in boldface $\boldsymbol{v}$ or by putting an arrow above the letter $\vec{v}$.

For instance, suppose a particle moves along a line segment from point $A$ to point $B$. The corresponding **displace ment vector $\boldsymbol{v}$** has **initial point** $A$ and **terminal point** $B$ and we indicate this by writing $\boldsymbol{v}=\vec{AB}$

We say that $\boldsymbol{u}$ and $\boldsymbol{v}$ are **equivalent** (or **equal**) and we write $\boldsymbol{u}=\boldsymbol{v}$

The **zero vector**, denote by $\boldsymbol{0}$, has length 0. It is the only vector with no specific direction.

**Definition of Vector Addition**: If $\boldsymbol{u}$ and $\boldsymbol{v}$ are vectors positioned so the initial point of $\boldsymbol{v}$ is at the terminal point of $\boldsymbol{u}$, then the **sum** $\boldsymbol{u}+\boldsymbol{v}$ is the vector from the initial point of $\boldsymbol{u}$ to the bermiinal point of $\boldsymbol{v}$.

<img src="/Users/hasson/Library/CloudStorage/OneDrive-InternationalCampus,ZhejiangUniversity/2025_FA_Semester/MATH 241/Notes/assets/image-20250916114607268.png" alt="image-20250916114607268" style="zoom:40%;" />

**Parallelogram Law**: If we place $\boldsymbol{u}$ and $\boldsymbol{v}$ so they start at the same point, then $\boldsymbol{u}+\boldsymbol{v}$ lies along the diagonal of the parallelogram with $\boldsymbol{u}$ and $\boldsymbol{v}$ as sides.

<img src="/Users/hasson/Library/CloudStorage/OneDrive-InternationalCampus,ZhejiangUniversity/2025_FA_Semester/MATH 241/Notes/assets/image-20250916114742442.png" alt="image-20250916114742442" style="zoom:40%;" />

**Definition of Scalar Multiplication**: If $c$ is a scalar and $\boldsymbol{v}$ is a vector, then the **scalar multiple** $c\boldsymbol{v}$ is the vector whose length is $|c|$ times the length of $\boldsymbol{v}$ and whose direction is the same as $\boldsymbol{v}$ if $c>0$ and is opposite to $\boldsymbol{v}$ if $c<0$. If $c=0$ or $\boldsymbol{v}=\boldsymbol{0}$, then $c\boldsymbol{v}=\boldsymbol{0}$.

### Components of a Vector

For some purposes it's best to introduce a coordinate system and treat vectors algebraically.

If we place the initial point of a vector $\boldsymbol{a}$ at the origin of a rectangular coordinate system, then the terminal point of a has coordinates of the form $(a_1,a_2)$ or $(a_1,a_2,a_3)$, depending on whether coordinate system is 2 or 3 dimensional.

These coordinates are called the **components** of $\boldsymbol{a}$ and we write
$$
\boldsymbol{a}=\langle a_1,a_2 \rangle \quad\text{or}\quad\boldsymbol{a}=\langle a_1,a_2,a_3\rangle
$$
We use the notation $\langle a_1,a_2\rangle$ for the ordered pair that refers to a vector so as not to confuse it with the ordered pair $(a_1,a_2)$ that refers to a point in the plane.

In three dimensions, the vector $\boldsymbol{a}=\vec{OP}=\langle a_1,a_2,a_3 \rangle$ is the **position vector** of the point $P(a_1,a_2,a_3)$.

<img src="/Users/hasson/Library/CloudStorage/OneDrive-InternationalCampus,ZhejiangUniversity/2025_FA_Semester/MATH 241/Notes/assets/image-20250918110357458.png" alt="image-20250918110357458" style="zoom:40%;" />

Given the points $A(x_1,y_1,z_1)$ and $B(x_2,y_2,z_2)$, the vector $\boldsymbol{a}$ with representation $\vec{AB}$ is
$$
\boldsymbol{a} = \langle x_2-x_1,y_2-y_1,z_2-z_1 \rangle
$$
The **magnitude** or **length** of the vector $\boldsymbol{v}$ is the length of any of itsrepresentations and is denoted by the symbol $|\boldsymbol{v}|$ or $\|\boldsymbol{v}\|$. By using the distance formula to compute the length of a segment $OP$, we obtain the following formulas.

The length of the $n$-dimensional vector $\boldsymbol{a}=\langle a_1,\dots,a_n \rangle$ is
$$
|\boldsymbol{a}| = \sqrt{\sum_{i=1}^na_{i}^2}
$$
We denote by $V_2$, the set of all two-dimensional vectors and by $V_3$, the set of allthree-dimensiona  vectors. More generally, we will consider the set $V_n$, of all $n$-dimensional vectors.

Three vectors in $V_3$ play a special role. Let
$$
\boldsymbol{i} = \langle1,0,0\rangle\quad\boldsymbol{j} = \langle0,1,0\rangle\quad \boldsymbol{k} = \langle0,0,1\rangle
$$
These vectors $\boldsymbol{i,j,k}$ are called the standard basis vectors. They have length 1 and point in the directions of the positive $x,y,z$-axes.

A **unit vector** is a vector whose length is 1. For instance, $\boldsymbol{i,j,k}$ are all unit vectors. In general, if $\boldsymbol{a}\ne0$, then the unit vector that has the same direction as $\boldsymbol{a}$ is
$$
\boldsymbol{u}=\frac{\boldsymbol{a}}{|\boldsymbol{a}|}
$$
In order to verify this, we let $c=\frac{1}{|\boldsymbol{a}|}$. Then $\boldsymbol{u}=c\boldsymbol{a}$ and $c$ is a positive scalar, so $\boldsymbol{u}$ has the same direction as $\boldsymbol{a}$.

## The Dot Product

### Dot Product of Two Vectors

To find the dot product of vectors $\boldsymbol{a}$ and $\boldsymbol{b}$ we multiply correspondingcomponents and add.

#### Definition

If $\boldsymbol{a}=\langle a_1,a_2,a_3 \rangle$ and $\boldsymbol{b}=\langle b_1,b_2,b_3 \rangle$, then the **dot product** of $\boldsymbol{a}$ and $\boldsymbol{b}$ is the number $\boldsymbol{a}\cdot\boldsymbol{b}$ given by
$$
\boldsymbol{a}\cdot\boldsymbol{b}=a_1b_1+a_2b_2+a_3b_3
$$

#### Properties

If $\boldsymbol{a}$, $\boldsymbol{b}$ and $\boldsymbol{c}$ are vectors in $V_3$ and $c$ is a scalar, then
$$
\begin{aligned}
\boldsymbol{a}\cdot\boldsymbol{a}&=|a|^2
\\
\boldsymbol{a}\cdot\boldsymbol{b} &= \boldsymbol{b}\cdot\boldsymbol{a}
\\
\boldsymbol{a}\cdot(\boldsymbol{b}+\boldsymbol{c}) &= \boldsymbol{a}\cdot\boldsymbol{b}+\boldsymbol{a}\cdot\boldsymbol{c}
\\
(c\boldsymbol{a})\cdot(\boldsymbol{b})&=c(\boldsymbol{a}\cdot\boldsymbol{b})=\boldsymbol{a}\cdot(c\boldsymbol{b})
\\
\boldsymbol{0}\cdot\boldsymbol{a}&=0
\end{aligned}
$$

#### Theorem

If $\theta$ is the angle between the vectors $\boldsymbol{a}$ and $\boldsymbol{b}$, then 
$$
\begin{aligned}
\boldsymbol{a}\cdot\boldsymbol{b}&=|\boldsymbol{a}||\boldsymbol{b}|\cos\theta
\\
\cos\theta&=\frac{\boldsymbol{a}\cdot\boldsymbol{b}}{|\boldsymbol{a}||\boldsymbol{b}|}
\end{aligned}
$$

#### Perpendicular or Orthogonal

Two nonzero vectors $\boldsymbol{a}$ and $\boldsymbol{b}$ are called **perpendicular** or **orthogonal** if the angle between them is $\theta=\frac{\pi}{2}$. Then the theorem gives
$$
\boldsymbol{a}\cdot\boldsymbol{b}=|\boldsymbol{a}||\boldsymbol{b}|\cos\left( \frac{\pi}{2} \right)=0
$$
and conversely if $\boldsymbol{a}\cdot\boldsymbol{b}=0$, then $\cos\theta=0$, so $\theta=\frac{\pi}{2}$. The zero vector $\boldsymbol{0}$ is considered to be perpendicular to all vectors. Therefore we have the following method for determining whether two vectors are orthogonal:
$$
\boldsymbol{a}\perp\boldsymbol{b} \equiv \boldsymbol{a}\cdot\boldsymbol{b}=0
$$

### Direction Angles and Direction Cosines

The **direction angles** of a nonzero vector $\boldsymbol{a}$ are the angles $\alpha,\beta,\gamma$ (in the interval $[0,\pi]$) that $\boldsymbol{a}$ makes with the positive $x,y,z$-axes, respectively.

<img src="/Users/hasson/Library/CloudStorage/OneDrive-InternationalCampus,ZhejiangUniversity/2025_FA_Semester/MATH 241/Notes/assets/image-20250918114710173.png" alt="image-20250918114710173" style="zoom:40%;" />

The cosines of these direction angles, $\cos\alpha,\cos\beta,\cos\gamma$ are called the **direction cosines** of the vector $\boldsymbol{a}$.
$$
\begin{aligned}
&\cos\alpha=\frac{\boldsymbol{a}\cdot\boldsymbol{i}}{|\boldsymbol{a}||\boldsymbol{i}|}=\frac{\boldsymbol{a}_1}{|\boldsymbol{a}|}
\\[10pt]
&\cos\beta=\frac{\boldsymbol{a}\cdot\boldsymbol{j}}{|\boldsymbol{a}||\boldsymbol{j}|}=\frac{\boldsymbol{a}_2}{|\boldsymbol{a}|}
\\[10pt]
&\cos\gamma=\frac{\boldsymbol{a}\cdot\boldsymbol{z}}{|\boldsymbol{a}||\boldsymbol{z}|}=\frac{\boldsymbol{a}_3}{|\boldsymbol{a}|}
\\[10pt]
&\cos^2\alpha+\cos^2\beta+\cos^2\gamma=1
\end{aligned}
$$

### Projections

If $S$ is the foot of the perpendicular from $R$ to the line containing $\vec{PQ}$, then the vector with representation $\vec{PS}$ is called the **vector projection** of $\boldsymbol{b}$ onto $\boldsymbol{a}$ and is denoted by $\text{proj}_{\boldsymbol{a}}\boldsymbol{b}$

<img src="/Users/hasson/Library/CloudStorage/OneDrive-InternationalCampus,ZhejiangUniversity/2025_FA_Semester/MATH 241/Notes/assets/image-20250923103600043.png" alt="image-20250923103600043" style="zoom:40%;" />

The **scalar projection** of $\boldsymbol{b}$ onto $\boldsymbol{a}$ (also called the **component of $\boldsymbol{b}$ along $\boldsymbol{a}$**) is defined to be the signed magnitude of the vector projection, which is the number $|\boldsymbol{b}|\cos{\theta}$, where $\theta$ is the angle between $\boldsymbol{a}$ and $\boldsymbol{b}$. This is denoted by $\text{comp}_{\boldsymbol{a}}\boldsymbol{b}$. Observe that it's negative if $\frac{\pi}{2}\lt\theta\le\pi$. 

<img src="/Users/hasson/Library/CloudStorage/OneDrive-InternationalCampus,ZhejiangUniversity/2025_FA_Semester/MATH 241/Notes/assets/image-20250923103826343.png" alt="image-20250923103826343" style="zoom:25%;" />

The equation
$$
\boldsymbol{a}\cdot\boldsymbol{b}=|\boldsymbol{a}||\boldsymbol{b}|\cos\theta=|\boldsymbol{a}|(|\boldsymbol{b}|\cos\theta)
$$
Shows that the dot product of $\boldsymbol{a}$ and $\boldsymbol{b}$ can be interpreted as the length of $\boldsymbol{a}$ times the scalar projection of $\boldsymbol{b}$ onto $\boldsymbol{a}$. Since
$$
|\boldsymbol{b}|\cos\theta=\frac{\boldsymbol{a}\cdot\boldsymbol{b}}{|\boldsymbol{a}|}=\frac{\boldsymbol{a}}{|\boldsymbol{a}|}\cdot\boldsymbol{b}
$$
the component of $\boldsymbol{b}$ along $\boldsymbol{a}$ can be computed by taking the dot product of $\boldsymbol{b}$ with the unit vector in the direction of $\boldsymbol{a}$

We summarize these ideas as follows:

- Scalar projection of $\boldsymbol{b}$ onto $\boldsymbol{a}$: $\text{comp}_{\boldsymbol{a}}\boldsymbol{b}=\frac{\boldsymbol{a}\cdot\boldsymbol{b}}{|\boldsymbol{a}|}$

- Vector projection of $\boldsymbol{b}$ onto $\boldsymbol{a}$: $\text{proj}_{\boldsymbol{a}}\boldsymbol{b}=\left(\text{comp}_{\boldsymbol{a}}\boldsymbol{b} \right)\frac{\boldsymbol{a}}{|\boldsymbol{a}|}=\frac{\boldsymbol{a}\cdot\boldsymbol{b}}{|\boldsymbol{a}|^2}\boldsymbol{a}$

## Cross Product (Vector Product)

### Cross Product of 2 Vectors

**Definition of the Cross Product**: If $\boldsymbol{a}=\langle a_1,a_2,a_3 \rangle$ and $\boldsymbol{b}=\langle b_1,b_2,b_3 \rangle$, then the **cross product** of $\boldsymbol{a}$ and $\boldsymbol{b}$ is the vector
$$
\boldsymbol{a}\times\boldsymbol{b}=\langle a_2b_3-a_3b_2,a_3b_1-a_1b_3,a_1b_2-a_2b_1 \rangle
$$
Notice that the **cross product** $\boldsymbol{a}\times\boldsymbol{b}$ of two vectors $\boldsymbol{a}$ and $\boldsymbol{b}$ is the vector. For this reason it's also called the **vector product**.

A **determinant of order 3** can be defined in terms of second-order determinants
$$
\begin{vmatrix}
\boldsymbol{i}&\boldsymbol{j}&\boldsymbol{k}\\
a_1&a_2&a_3\\
b_1&b_2&b_3
\end{vmatrix}
=\begin{vmatrix}
a_2&a_3\\
b_2&b_3
\end{vmatrix}\boldsymbol{i}
-\begin{vmatrix}
a_1&a_3\\
b_1&b_3
\end{vmatrix}\boldsymbol{j}
+\begin{vmatrix}
a_2&a_3\\
b_12&b_3
\end{vmatrix}\boldsymbol{k}
$$
That is the cross product of two vectors $\boldsymbol{a}$ and $\boldsymbol{b}$

### Properties of the Cross Product

#### Orthogonality

The vector $\boldsymbol{a}\times\boldsymbol{b}$ is orthogonal to both $\boldsymbol{a}$ and $\boldsymbol{b}$. This can be easily proved by dot product.

If $\boldsymbol{a}$ and $\boldsymbol{b}$ are represented by directed line segments with the same initial point, then the cross product $\boldsymbol{a}\times\boldsymbol{b}$ points in a direction perpendicular to the plane through $\boldsymbol{a}$ and $\boldsymbol{b}$.

<img src="/Users/hasson/Library/CloudStorage/OneDrive-InternationalCampus,ZhejiangUniversity/2025_FA_Semester/MATH 241/Notes/assets/image-20250923110936645.png" alt="image-20250923110936645" style="zoom:25%;" />

#### Magnitude

If $\theta$ is the angle between $\boldsymbol{a}$ and $\boldsymbol{b}$ (so $0\le\theta\le\pi$), then the length of the cross product $\boldsymbol{a}\times\boldsymbol{b}$ is given by
$$
|\boldsymbol{a}\times\boldsymbol{b}|=|\boldsymbol{a}||\boldsymbol{b}|\sin\theta
$$
This leads to a corollary: 2 nonzero vectors $\boldsymbol{a}$ and $\boldsymbol{b}$ are parallel if and only if
$$
\boldsymbol{a}\times\boldsymbol{b}=\boldsymbol{0}
$$
Since a vector is completely determined by its magnitude and direction, we can now say that for nonparallel vectors $\boldsymbol{a}$ and $\boldsymbol{b}$, $\boldsymbol{a}\times\boldsymbol{b}$ is the vector that is perpendicular to both $\boldsymbol{a}$ and $\boldsymbol{b}$, whose orientation is determined by the right-hand rule, and whose length is $|\boldsymbol{a}||\boldsymbol{b}|\sin\theta$.

#### Geometric Interpretation

<img src="/Users/hasson/Library/CloudStorage/OneDrive-InternationalCampus,ZhejiangUniversity/2025_FA_Semester/MATH 241/Notes/assets/image-20250923111545933.png" alt="image-20250923111545933" style="zoom:35%;" />

If $\boldsymbol{a}$ and $\boldsymbol{b}$ are represented by directed line segments with the same initial point, then they determined a parallelogram with base $|\boldsymbol{a}|$, altitude $|\boldsymbol{b}|\sin\theta$, and area
$$
A=|\boldsymbol{a}|(|\boldsymbol{b}|\sin\theta)=|\boldsymbol{a}\times\boldsymbol{b}|
$$
Thus we have the following way of interpreting the magnitude of a cross product. The length of the cross product $\boldsymbol{a}\times\boldsymbol{b}$ is equal to the area of the parallelogram determined by $\boldsymbol{a}$ and $\boldsymbol{b}$.

#### Others

If $\boldsymbol{a}$, $\boldsymbol{b}$ and $\boldsymbol{c}$ are vectors and $c$ is a scalar, then
$$
\begin{aligned}
\boldsymbol{a}\times\boldsymbol{b}&=-\boldsymbol{b}\times\boldsymbol{a}
\\[10pt]
(c\boldsymbol{a})\times\boldsymbol{b}&=c(\boldsymbol{a}\times\boldsymbol{b})=\boldsymbol{a}\times(c\boldsymbol{b})
\\[10pt]
\boldsymbol{a}\times(\boldsymbol{b}+\boldsymbol{c})&=\boldsymbol{a}\times\boldsymbol{b}+\boldsymbol{a}\times\boldsymbol{c}
\\[10pt]
(\boldsymbol{a}+\boldsymbol{b})\times\boldsymbol{c}&=\boldsymbol{a}\times\boldsymbol{c}+\boldsymbol{b}\times\boldsymbol{c}
\\[10pt]
\boldsymbol{a}\cdot(\boldsymbol{b}\times\boldsymbol{c})&=(\boldsymbol{a}\times\boldsymbol{b})\cdot\boldsymbol{c}
\\[10pt]
\boldsymbol{a}\times(\boldsymbol{b}\times\boldsymbol{c})&=(\boldsymbol{a}\cdot\boldsymbol{c})\boldsymbol{b}-(\boldsymbol{a}\cdot\boldsymbol{b})\boldsymbol{c}
\end{aligned}
$$

### Triple Products

The product $\boldsymbol{a}\cdot(\boldsymbol{b}\times\boldsymbol{c})$ is called the **scalar triple product** of the vectors $\boldsymbol{a}$, $\boldsymbol{b}$ and $\boldsymbol{c}$. We can write the scalar triple product as a determinant:
$$
\boldsymbol{a}\cdot(\boldsymbol{b}\times\boldsymbol{c})=
\begin{vmatrix}
a_1&a_2&a_3\\
b_1&b_2&b_3\\
c_1&c_2&c_3
\end{vmatrix}
$$
The geometric significance of the scalar triple product can be seen by considering the parallelpiped determined by the vectors $\boldsymbol{a}$, $\boldsymbol{b}$ and $\boldsymbol{c}$.

<img src="/Users/hasson/Library/CloudStorage/OneDrive-InternationalCampus,ZhejiangUniversity/2025_FA_Semester/MATH 241/Notes/assets/image-20250923115055632.png" alt="image-20250923115055632" style="zoom:40%;" />

If $\theta$ is the angle between $\boldsymbol{a}$ and $\boldsymbol{b}\times\boldsymbol{c}$, then the height $h$ of the parallelepiped is $h=|\boldsymbol{a}||\cos\theta|$. Therefore, the volume of the parallelepiped is
$$
V=Ah=|\boldsymbol{b}\times\boldsymbol{c}||\boldsymbol{a}||\cos\theta|=|\boldsymbol{a}\cdot(\boldsymbol{b}\times\boldsymbol{c})|
$$
If the volume of the parallelepiped determined by $\boldsymbol{a}$, $\boldsymbol{b}$ and $\boldsymbol{c}$ is 0, then the vectors must lie in the same plane; that is, they are **coplanar**.

## Equations of Lines and Planes

### Lines

A line $L$ in three-dimensional space is determined when we know a point $P_0(x_0,y_0,z_0)$ on $L$ and the direction of $L$, which is conveniently described by a vector $\boldsymbol{v}$ parallel to the line. Let $P(x,y,z)$ be an arbitrary point on $L$ and let $\boldsymbol{r}_0$ and $\boldsymbol{r}$ be the position vectors of $P_0$ and $P$. If $\boldsymbol{a}$ is the vector with representation $\vec{P_0P}$, then the Triangle Law for vector addition gives $\boldsymbol{r}=\boldsymbol{r_0}+\boldsymbol{a}$. Since $\boldsymbol{a}$ and $\boldsymbol{v}$ are parallel vectors, there is a scalar $t$ such that $\boldsymbol{a}=t\boldsymbol{v}$. Thus
$$
\boldsymbol{r}=\boldsymbol{r}_0+t\boldsymbol{v}
$$
which is a **vector equation** of $L$. Each value of the **parameter** $t$ gives the position vector $\boldsymbol{r}$ of a point on $L$. In other words, as $t$ varies, the line is traced out by the tip of the vector $\boldsymbol{r}$.

Therefore we have the three scalar equations
$$
x=x_0+at\quad y=y_0+bt\quad z=z_0+ct
$$
These equations are called **parametric equations** of the line $L$ through the point $P_0(x_0,y_0,z_0)$ and parallel to the vector $\boldsymbol{v}=\langle a,b,c \rangle$. Each value of the parameter $t$ gives a point $(x,y,z)$ on $L$.

In general, if a vector $\boldsymbol{v}=\langle a,b,c \rangle$ is used to describe the direction of a line $L$, then the numbers $a,b,c$ are called **direction numbers** of $L$. 

If none of $a,b,c$ is 0, we can solve each of these equations for $t$:
$$
t=\frac{x-x_0}{a}=\frac{y-y_0}{b}=\frac{z-z_0}{c}
$$
These equations are called **symmetric equations** of $L$. 

If one of $a,b,c$ is 0, we can still eliminate $t$. For instance, if $a=0$, we could write the equation of $L$ as
$$
x=x_0,\quad \frac{y-y_0}{b}=\frac{z-z_0}{c}
$$
This means that $L$ lies in the vertical plane $x=x_0$.

### Planes

A plane in space is determined by a point $P_0(x_0,y_0,z_0)$ in the plane and a vector $\boldsymbol{n}$ that is orthogonal to the plane. This orthogonal vector $\boldsymbol{n}$ is called a **normal vector**. Let $P(x,y,z)$ be an arbitrary point in the plane, and let $\boldsymbol{r}_0$ and $\boldsymbol{r}$ be the position vectors of $P_0$ and $P$. Then the vector $\boldsymbol{r}-\boldsymbol{r}_0$ is represented by $\vec{P_0P}$. The normal vector $\boldsymbol{n}$ is orthogonal to every vector in the given plane. In particular, $\boldsymbol{n}$ is orthogonal to $\boldsymbol{r}-\boldsymbol{r}_0$ and so we have
$$
\boldsymbol{n}\cdot(\boldsymbol{r}-\boldsymbol{r}_0)=0
$$
which can be written as
$$
\boldsymbol{n}\cdot\boldsymbol{r}=\boldsymbol{n}\cdot\boldsymbol{r}_0
$$
This is called a **vector equation of the plane**.

To obtain a scalar for the plane, we write
$$
\boldsymbol{n}=\langle a,b,c \rangle,\quad\boldsymbol{r}=\langle x,y,z \rangle,\quad \boldsymbol{r}_0=\langle x_0,y_0,z_0 \rangle
$$
Then the vector equation becomes
$$
\langle a,b,c \rangle\cdot\langle x-x_0,y-y_0,z-z_0 \rangle=0
$$
A **scalar equation of the plane** through point $P_0(x_0,y_0,z_0)$ with normal vector $\boldsymbol{n}=\langle z,b,c \rangle$ is
$$
a(x-x_0)+b(y-y_0)+c(z-z_0)=0
$$
We can rewrite the equation of a plane as
$$
ax+by+cz+d=0
$$
where $d=-(ax_0+by_0+cz_0)$. This is called a **linear equation** in $x,y,z$. Conversely, it can bes hown that if $a,b,c$ are not all 0, then the linear equation represents a plane with normal vector $\langle a,b,c \rangle$. 

Two planes are **parallel** if their normal vectors are parallel. If two planes are not parallel, then they intersect in a straight line and the angle between the two planes is defined as the acute angle between their normal vectors.

### Distances

Find a formula for the distance $D$ from a point $P_1(x_1,y_1,z_1)$ to the plane $ax+by+cz+d=0$. Let $P_0(x_0,y_0,z_0)$ be any point in the given plane and let $\boldsymbol{b}$ be the vector corresponding to $\vec{P_0P_1}$. Then
$$
\boldsymbol{b}=\langle x_1-x_0,y_1-y_0,z_1-z_0 \rangle
$$
The distance $D$ from $P_1$ to the plane is equal to the absolute value of the scalar projection of $\boldsymbol{b}$ onto the normal vector $\boldsymbol{n}=\langle a,b,c \rangle$. Thus
$$
\begin{aligned}
D&=|\text{comp}_{\boldsymbol{n}}\boldsymbol{b}|=\frac{\boldsymbol{n}\cdot\boldsymbol{b}}{|\boldsymbol{n}|}
\\[10pt]
&=\frac{|a(x_1-x_0)+b(x_1-x_0)+c(z_1-z_0)|}{\sqrt{a^2+b^2+c^2}}
\\[10pt]
&=\frac{(ax_1+by_1+cz_1)-(ax_0+by_0+cz_0)}{\sqrt{a^2+b^2+c^2}}
\end{aligned}
$$
Since $P_0$ lies in the plane, its coordinates satisfy the equation of the plane and so we have
$$
ax_0+by_0+cz_0+d=0
$$
Thus the distance $D$ from the point $P_1(x_1,y_1,z_1)$ to the plane $ax+by+cz+d=0$ is
$$
D=\frac{|ax_1+by_1+cz_1+d|}{\sqrt{a^2+b^2+c^2}}
$$

## Cylinders and Quadric Surfaces

In order to sketch the graph of a surface, it is useful to determine the curves of intersection of the surface with planes parallel to the coordinate planes. These curves are called **traces** (or cross-sections) of the surface.

### Cylinder

A **cylinder** is a surface that consists of all lines (called **rulings**) that are parallel to a given line and pass through a given plane curve.

If one of the variables $x,y,z$ is missing from the equation of a surface, then the surface is a cylinder. When you are dealing with surfaces, it is important to recognize that an equation like $x^2+y^2=1$ represents a cylinder and not a circle. The trace of the cylinder $x^2+y^2=1$ in the $xy$-plane is the circle with equations $x^2+y^2=1,z=0$.

### Quadric Surfaces

A **quadric surface** is the graph of a second-degree equation in three variables $x,y,z$. The most general such equation is 
$$
Ax^2+By^2+Cz^2+Dxy+Eyz+Fxz+Gx+Hy+Iz+J=0
$$
where $A,B,\dots,J$ are constants, but by translation and rotation it can be brought into one of the two standard forms
$$
Ax^2+By^2+Cz^2+J=0\quad\text{or}\quad Ax^2+By^2+Iz=0
$$
Quadric surfaces are the counterparts in three dimensions of the conic sections in the plane.

The idea of using traces to draw a surface is employed in three-dimensional graphing software. In most such software, traces in the vertical planes $x=k$ and $y=k$ are drawn for equally spaced values of $k$.

All surfaces are symmetric with respect to the $z$-axis. lf a quadric surface is symmetric about a different axis, its equation changes accordingly.