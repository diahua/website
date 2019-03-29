## Ray Tracer

### Adaptive Anti-Aliasing
Adaptive anti-aliasing is used to remove jaggies only at pixels whose intensity differs from its neighbors by some threshold.

![Image](nonhier_anti_alias.png)

### Soft Shadows 
Shadow rays are distributed across the light source to create the appearance of soft shadows.

![Image](nonhier_soft.png)

### Bump Mapping
Bump mapping is implemented by using a height displacement to calculate perturbed normals, creating a bumpy or wrinkled appearance.

![Image](simple_bump.png)

### Texture Mapping
Texture mapping is implemented for spheres, cubes, and meshes.

![Image](simple_texture.png)
![Image](spot_textured.png)

### Depth of Field
A focal length and aperture can be specified to produce a depth of field effect.

![Image](nonhier_dof_700_20_32.png)

### Reflection
Reflection is implemented for reflective objects, recursively casting a secondary ray in the direction of reflection.

![Image](nonhier_reflection.png)

### Refraction
Refraction is implemented for translucent objects, recursively casting a secondary ray in the direction of transmission given by Snell's law.

![Image](simple-cows_refract_1.01.png)

### Glossy Reflection
Multiple reflection rays are pertubed from the angle of reflection to create glossy reflection.

![Image](nonhier_glossy_reflection_64_0.1.png) 

### Glossy Refraction
Multiple refraction rays are perturbed from the angle of refraction to create glossy refraction. Fresnel's law is used to ...

![Image](simple-cows_glossy_refract_4.png)
![Image](simple-cows_glossy_refract_64.png)

### Extra Objective: Phong Shading
Barycentric coordinates are used to interpolate normal vectors.

![Image](bob_no_phong.png) 
![Image](bob_phong.png)

### Final Scene
A unique final scene is created which demonstrates the graphical objectives of the ray tracer.