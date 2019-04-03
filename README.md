## Ray Tracer

### Adaptive Anti-Aliasing
Adaptive anti-aliasing is used to remove jaggies only at pixels whose intensity differs from its neighbors by some threshold.

<figure>
  <img src="antialiasing/no_antialias.png" alt="my alt text" width="256" height="256"/>
  <figcaption>No antialiasing.</figcaption>
</figure>
<figure>
  <img src="antialiasing/antialias_border.png" alt="my alt text" width="256" height="256"/>
  <figcaption>No antialiasing.</figcaption>
</figure>
<figure>
  <img src="antialiasing/antialias.png" alt="my alt text" width="256" height="256"/>
  <figcaption>No antialiasing.</figcaption>
</figure>

### Soft Shadows 
Shadow rays are distributed across the light source to create the appearance of soft shadows.

<img src="shadows/ref.png" alt="image" width="256" height="256"/>
<img src="shadows/soft.png" alt="image" width="256" height="256"/>

### Bump Mapping
Bump mapping is implemented by using a height displacement to calculate perturbed normals, creating a bumpy or wrinkled appearance.

<img src="bump/simple_bump2.png" alt="image" width="256" height="256"/>
<img src="bump/simple_bump3.png" alt="image" width="256" height="256"/>

### Texture Mapping
Texture mapping is implemented for spheres, cubes, and meshes.

<img src="texture/simple_texture.png" alt="image" width="256" height="256"/>
<img src="texture/spot_textured.png" alt="image" width="256" height="256"/>

### Depth of Field
A focal length and aperture can be specified to produce a depth of field effect.

<img src="dof/nonhier2_dof_700_20_64.png" alt="image" width="256" height="256"/>
<img src="dof/nonhier2_dof_900_20_32.png" alt="image" width="256" height="256"/>
<img src="dof/nonhier2_dof_1100_20_32.png" alt="image" width="256" height="256"/>

### Reflection
Reflection is implemented for reflective objects, recursively casting a secondary ray in the direction of reflection.

<img src="reflection/nonhier2.png" alt="image" width="256" height="256"/>
<img src="reflection/nonhier2_refcolor.png" alt="image" width="256" height="256"/>

### Refraction
Refraction is implemented for translucent objects, recursively casting a secondary ray in the direction of transmission given by Snell's law.

<img src="refraction/simple-cows_refract_1.01.png" alt="image" width="256" height="256"/>
<img src="refraction/simple-cows_refract_1.33.png" alt="image" width="256" height="256"/>

### Glossy Reflection
Multiple reflection rays are pertubed from the angle of reflection to create glossy reflection.

<img src="reflection/nonhier2.png" alt="image" width="256" height="256"/>
<img src="glossy_reflection/nonhier_glossy_reflection_64_0.05.png" alt="image" width="256" height="256"/>

### Glossy Refraction
Multiple refraction rays are perturbed from the angle of refraction to create glossy refraction. Fresnel's law is used to ...

<img src="refraction/simple-cows_refract_1.01.png" alt="image" width="256" height="256"/>
<img src="glossy_refraction/simple-cows_glossy_refract_4_512_2.png" alt="image" width="256" height="256"/>
<img src="glossy_refraction/simple-cows_glossy_refract_64.png" alt="image" width="256" height="256"/>

### Extra Objective: Phong Shading
Barycentric coordinates are used to interpolate normal vectors.

<img src="phong/bob_no_phong.png" alt="image" width="256" height="256"/>
<img src="phong/bob_phong.png" alt="image" width="256" height="256"/>

### Final Scene
A unique final scene is created which demonstrates the graphical objectives of the ray tracer.

![Image](scene/scene30.png)