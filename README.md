## Ray Tracer

### Adaptive Anti-Aliasing
Adaptive anti-aliasing is used to remove jaggies only at pixels whose intensity differs from its neighbors by some threshold.

| <img src="antialiasing/no_antialias.png" alt="my alt text" width="256" height="256"/>  |  <img src="antialiasing/antialias_border.png" alt="my alt text" width="256" height="256"/> |   <img src="antialiasing/antialias.png" alt="my alt text" width="256" height="256"/> |
| Image without antialiasing  | Resampled pixels  | Antialiased image |

### Soft Shadows 
Shadow rays are distributed across the light source to create the appearance of soft shadows.

| <img src="shadows/ref.png" alt="my alt text" width="256" height="256"/>  |  <img src="shadows/soft.png" alt="my alt text" width="256" height="256"/> |
| Hard shadows  | Soft shadows |


### Bump Mapping
Bump mapping is implemented by using a height displacement to calculate perturbed normals, creating a bumpy or wrinkled appearance.

| <img src="bump/simple_bump2.png" alt="my alt text" width="256" height="256"/>  |  <img src="bump/simple_bump3.png" alt="my alt text" width="256" height="256"/> |
| Light from the right side  | Light from the left side |

### Texture Mapping
Texture mapping is implemented for spheres, cubes, and meshes.

| <img src="texture/simple_texture.png" alt="my alt text" width="256" height="256"/>  |  <img src="texture/spot_textured.png" alt="my alt text" width="256" height="256"/> |
| Textured primitives  | Textured triangular mesh |

### Depth of Field
A focal length and aperture can be specified to produce a depth of field effect.

| <img src="dof/nonhier2_dof_700_20_64.png" alt="my alt text" width="256" height="256"/>  |  <img src="dof/nonhier2_dof_900_20_32.png" alt="my alt text" width="256" height="256"/> |   <img src="dof/nonhier2_dof_1100_20_32.png" alt="my alt text" width="256" height="256"/> |
| Focal length of 700 | Focal length of 900 | Focal length of 1100 |

### Reflection
Reflection is implemented for reflective objects, recursively casting a secondary ray in the direction of reflection.

| <img src="reflection/nonhier2.png" alt="my alt text" width="256" height="256"/>  |  <img src="reflection/nonhier2_refcolor.png" alt="my alt text" width="256" height="256"/> |
| Mirror reflection | Colored reflection |

### Refraction
Refraction is implemented for translucent objects, recursively casting a secondary ray in the direction of transmission given by Snell's law.

| <img src="refraction/simple-cows_refract_1.01.png" alt="my alt text" width="256" height="256"/>  |  <img src="refraction/simple-cows_refract_1.33.png" alt="my alt text" width="256" height="256"/> |
| Refraction index of 1.01 | Refraction index of 1.33 |

### Glossy Reflection
Multiple reflection rays are pertubed from the angle of reflection to create glossy reflection.

| <img src="reflection/nonhier2.png" alt="my alt text" width="256" height="256"/>  |  <img src="glossy_reflection/nonhier_glossy_reflection_64_0.05.png" alt="my alt text" width="256" height="256"/> |
| Mirror reflection | Glossy reflection |

### Glossy Refraction
Multiple refraction rays are perturbed from the angle of refraction to create glossy refraction. Fresnel's law is used to ...

| <img src="refraction/simple-cows_refract_1.01.png" alt="my alt text" width="256" height="256"/>  |  <img src="glossy_refraction/simple-cows_glossy_refract_4_512_2.png" alt="my alt text" width="256" height="256"/> |   <img src="glossy_refraction/simple-cows_glossy_refract_64.png" alt="my alt text" width="256" height="256"/> |
| ------ | ------ | ------ |
| Normal refraction | Glossy refraction using 4 rays | Glossy refraction using 64 rays |

### Extra Objective: Phong Shading
Barycentric coordinates are used to interpolate normal vectors.

| <img src="phong/bob_no_phong.png" alt="my alt text" width="256" height="256"/>  |  <img src="phong/bob_phong.png" alt="my alt text" width="256" height="256"/> |
| No phong shading | Phong shading | 

### Final Scene
A unique final scene is created which demonstrates the graphical objectives of the ray tracer.

![Image](scene/scene30.png)