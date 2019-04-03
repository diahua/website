## Ray Tracer

### Adaptive Anti-Aliasing
Adaptive anti-aliasing is used to remove jaggies only at pixels whose intensity differs from its neighbors by some threshold.

![Image](antialiasing/no_antialias.png)
![Image](antialiasing/antialias_border.png)
![Image](antialiasing/antialias.png)

### Soft Shadows 
Shadow rays are distributed across the light source to create the appearance of soft shadows.

![Image](shadows/ref.png)
![Image](shadows/soft.png)

### Bump Mapping
Bump mapping is implemented by using a height displacement to calculate perturbed normals, creating a bumpy or wrinkled appearance.

![Image](bump/simple_bump2.png)
![Image](bump/simple_bump3.png)

### Texture Mapping
Texture mapping is implemented for spheres, cubes, and meshes.

![Image](texture/simple_texture.png)
![Image](texture/spot_textured.png)

### Depth of Field
A focal length and aperture can be specified to produce a depth of field effect.

![Image](dof/nonhier2_dof_700_20_64.png)
![Image](dof/nonhier2_dof_900_20_32.png)
![Image](dof/nonhier2_dof_1100_20_32.png)

### Reflection
Reflection is implemented for reflective objects, recursively casting a secondary ray in the direction of reflection.

![Image](reflection/nonhier2.png)
![Image](reflection/nonhier2_refcolor.png)

### Refraction
Refraction is implemented for translucent objects, recursively casting a secondary ray in the direction of transmission given by Snell's law.

![Image](refraction/simple-cows_refract_1.01.png)
![Image](refraction/simple-cows_refract_1.33.png)

### Glossy Reflection
Multiple reflection rays are pertubed from the angle of reflection to create glossy reflection.

![Image](reflection/nonhier2.png)
![Image](glossy_reflection/nonhier_glossy_reflection_64_0.05.png)

### Glossy Refraction
Multiple refraction rays are perturbed from the angle of refraction to create glossy refraction. Fresnel's law is used to ...

![Image](refraction/simple-cows_refract_1.01.png)
![Image](glossy_refraction/simple-cows_glossy_refract_4_512_2.png)
![Image](glossy_refraction/simple-cows_glossy_refract_64.png)

### Extra Objective: Phong Shading
Barycentric coordinates are used to interpolate normal vectors.

![Image](phong/bob_no_phong.png) 
![Image](phong/bob_phong.png)

### Final Scene
A unique final scene is created which demonstrates the graphical objectives of the ray tracer.

![Image](scene/scene30.png)