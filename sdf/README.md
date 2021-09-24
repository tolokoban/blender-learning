# How to do SDF?

Download the [Blender 2.93.4 file](sdf.blend).

![sdf.blend](sdf.webp)


SDF function for a donut is: `(√(x² + y²) - R²) + z² - r² < 0`.

1. Create a simple cube.
2. Remove the **Surface Shader** but add a **Volume Shader**. We will use the density of absorbtion volume.
  ![volume shader](step-2.webp)
3. All the maths are done with **Converter/Math** nodes.
  ![math](step-3.webp)
4. `x`, `y` and `z` have to be taken from **texture coordinates**
  ![texture coordinates](step-1.webp)

