To find the shadow of a 3D point on the \(z = 0\) plane under sunlight, we need to project the point onto the plane using the direction defined by the sun's azimuth and elevation angles.

### Definitions:
- **Sunlight direction**:
  - Azimuth (\(\theta\)): Angle from the north (clockwise in horizontal plane).
  - Elevation (\(\phi\)): Angle above the horizontal plane.
- **Point in space**: \(P(x_1, y_1, z_1)\) (the point casting the shadow).
- **Shadow point on \(z = 0\)**: \(S(x_s, y_s, 0)\) (the point where the shadow falls).

### Shadow Calculation:
The shadow is the intersection of the line through \(P\) in the direction of sunlight with the \(z = 0\) plane.

1. **Direction vector of sunlight**:
   \[
   \mathbf{d} = (\cos\phi \cdot \sin\theta, \cos\phi \cdot \cos\theta, -\sin\phi)
   \]

2. **Line equation**: A parametric line through \(P\) in the direction of \(\mathbf{d}\):
   \[
   (x, y, z) = (x_1, y_1, z_1) + t \cdot (\cos\phi \cdot \sin\theta, \cos\phi \cdot \cos\theta, -\sin\phi)
   \]
   Here, \(t\) is the parameter.

3. **Condition for intersection with \(z = 0\)**:
   \[
   z = z_1 - t \cdot \sin\phi = 0
   \]
   Solve for \(t\):
   \[
   t = \frac{z_1}{\sin\phi}
   \]

4. **Substitute \(t\) to get shadow coordinates**:
   \[
   x_s = x_1 + t \cdot \cos\phi \cdot \sin\theta
   \]
   \[
   y_s = y_1 + t \cdot \cos\phi \cdot \cos\theta
   \]
   Substitute \(t = \frac{z_1}{\sin\phi}\):
   \[
   x_s = x_1 + \frac{z_1}{\sin\phi} \cdot \cos\phi \cdot \sin\theta
   \]
   \[
   y_s = y_1 + \frac{z_1}{\sin\phi} \cdot \cos\phi \cdot \cos\theta
   \]

### Final Formulas:
\[
x_s = x_1 + z_1 \cdot \frac{\cos\phi \cdot \sin\theta}{\sin\phi}
\]
\[
y_s = y_1 + z_1 \cdot \frac{\cos\phi \cdot \cos\theta}{\sin\phi}
\]

### Notes:
- The result depends on the azimuth (\(\theta\)) and elevation (\(\phi\)) of the sunlight.
- \(x_s, y_s\) are the coordinates of the shadow on the horizontal plane (\(z = 0\)).
