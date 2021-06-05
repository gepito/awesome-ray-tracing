# Awesome Ray Tracing [![CC0 License](http://i.creativecommons.org/p/zero/1.0/88x31.png)](http://creativecommons.org/publicdomain/zero/1.0/)

A curated list of ray tracing resources.
PR's welcome!

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/32/Recursive_raytrace_of_a_sphere.png/240px-Recursive_raytrace_of_a_sphere.png" height="200"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/ec/Glasses_800_edit.png/320px-Glasses_800_edit.png" height="200"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/36/Ray-traced_steel_balls.jpg/320px-Ray-traced_steel_balls.jpg" height="200"><img src="https://upload.wikimedia.org/wikipedia/commons/0/0d/Global_illumination.JPG" height="200"><img src="https://upload.wikimedia.org/wikipedia/commons/c/cb/Alexexterior2.jpg" height="200"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e0/Path_tracing_001.png/240px-Path_tracing_001.png" height="200"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/40/Glass_ochem.png/640px-Glass_ochem.png" height="200"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/63/Glas-1000-enery.jpg/320px-Glas-1000-enery.jpg" height="200">

## Table of Contents

- [Glossary of Terms](GLOSSARY.md)
- [What is Ray Tracing?](#what-is-ray-tracing)
- [Iconic Publications](#iconic-publications)
- [Path Tracing](#path-tracing)
- [Photon Mapping](#photon-mapping)
- [Math](#math)
- [Ray Casting](#ray-casting)
- [BxDF](#bxdf)
- [Sampling Methods](#sampling-methods)
- [Denoising, Filtering, and Reconstruction](#denoising-filtering-and-reconstruction)
- [Realtime](#realtime)
- [Reference Scenes](#reference-scenes)
- [News](#news)
- [API's](#apis)
  - [Vulkan Ray Tracing](#vulkan-ray-tracing)
  - [Nvidia RTX](#nvidia-rtx)
  - [Microsoft DirectX Raytracing (RTX)](#microsoft-directx-raytracing-dxr)
  - [Nvidia OptiX](#nvidia-optix)
- [Applications](#applications)
  - [GLSL-PathTracer](#glsl-raytracer)
  
## Legend

| Icon | Meaning |
| ---- | ------- |
| 📖 | Reading |
| 📺 | Video |
| 💾 | Code / Asset |

---

## [Glossary of Terms](GLOSSARY.md)

## What is Ray Tracing?

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/83/Ray_trace_diagram.svg/320px-Ray_trace_diagram.svg.png" height="200">

- 📺 [Ray Tracing Essentials - (2020) *Eric Haines*](https://www.youtube.com/playlist?list=PL5B692fm6--sgm8Uiava0IIvUojjFOCSR)
- 📺 [Disney's Practical Guide to Path Tracing - (2016) *Disney*](https://youtu.be/frLwRLS_ZR0)
- 📖 [What’s the Difference Between Ray Tracing and Rasterization? - (2018) *Brian Caulfield*](https://blogs.nvidia.com/blog/2018/03/19/whats-difference-between-ray-tracing-rasterization/)
- 📖 [Ray Tracing Resources Page - (2018) *Tomas Akenine-Möller, Eric Haines, Naty Hoffman, Angelo Pesce, Michał Iwanicki, and Sébastien Hillaire*](http://www.realtimerendering.com/raytracing.html)
- 📖 [An Introduction to Ray Tracing - (1991) *Andrew Glassner*](http://www.realtimerendering.com/raytracing/An-Introduction-to-Ray-Tracing-The-Morgan-Kaufmann-Series-in-Computer-Graphics-.pdf)
- 📖 [Physically Based Rendering Book (PBR) - (2018) *Matt Pharr, Wenzel Jakob, Greg Humphreys, and Morgan Kaufmann*](http://www.pbr-book.org/)
- 📖 [Ray Tracing in One Weekend - (2016) *Peter Shirley*](http://in1weekend.blogspot.com/2016/01/ray-tracing-in-one-weekend.html)
  - 📖 [Ray Tracing: The Next Week - (2016) *Peter Shirley*](http://in1weekend.blogspot.com/2016/01/ray-tracing-second-weekend.html)
  - 📖 [Ray Tracing: The Rest of Your Life - (2016) *Peter Shirley*](http://in1weekend.blogspot.com/2016/03/ray-tracing-rest-of-your-life.html)
- 📺 [An Explanation of the Rendering Equation - (2019) *Eric Arnebäck*](https://www.youtube.com/watch?v=eo_MTI-d28s)
- 📺 [Ray Marching for Dummies! - (2018) *Martijn Steinrucken*](https://www.youtube.com/watch?v=PGtv-dBi2wE)
- 📺 [Rendering / Ray Tracing Course - (2017) *TU Wien*](https://www.youtube.com/playlist?list=PLujxSBD-JXgnGmsn7gEyN28P1DnRZG7qi)

## Iconic Publications

- 📖 [Some Techniques for Shading Machine Renderings of Solids - (1968) *Arthur Appel*](http://graphics.stanford.edu/courses/Appel.pdf)
- 📖 [An Improved Illumination Model for Shaded Display - (1979) * J.D. Foley and Turner Whitted*](http://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.156.1534)
- 📖 [The Rendering Equation - (1986) *James T. Kajiya*](http://www.dca.fee.unicamp.br/~leopini/DISCIPLINAS/IA725/ia725-12010/kajiya-SIG86-p143.pdf)
- 📖 [Robust Monte Carlo Methods for Light Transport Simulation (1998) - *Eric Veach*](https://graphics.stanford.edu/papers/veach_thesis/)
- 📖 [Global Illumination Compendium - (2003) *Philip Dutré*](https://people.cs.kuleuven.be/~philip.dutre/GI/TotalCompendium.pdf)


## Path Tracing

- 📖 [Path Tracing - (2017) *Fabio Pellacini and Steve Marschner*](http://pellacini.di.uniroma1.it/teaching/graphics17b/lectures/12_pathtracing.pdf)
- 📖 [Path Tracing in Production - (2018) *Luca Fascione, Johannes Hanika, Rob Pieké, Ryusuke Villemin, Christophe Hery, Manuel Gamito, Luke Emrose, and André Mazzone*](https://jo.dreggn.org/path-tracing-in-production/2018/index.html)
- 📖 [Path Tracing Coherency - *Anders Lindqvist*](https://www.breakin.se/learn/pathtracing-coherency.html)
- 📖 [Path Traced Depth of Field and Bokeh - (2018) *Alan Wolfe*](https://blog.demofox.org/2018/07/04/pathtraced-depth-of-field-bokeh/)
- 📖 [Daily Path Tracer - (2018) *Aras Pranckevičius*](http://aras-p.info/blog/2018/03/28/Daily-Pathtracer-Part-0-Intro/)
- 📖 [Microfacet-based Normal Mapping for Robust Monte Carlo Path Tracing - (2017) *Vincent Schüssler, Eric Heitz, Johannes Hanika, Carsten Dachsbacher*](https://jo.dreggn.org/home/2017_normalmap.pdf)

## Photon Mapping

- 📖 [Photon Mapping - *Zack Waters*](https://web.cs.wpi.edu/~emmanuel/courses/cs563/write_ups/zackw/photon_mapping/PhotonMapping.html)

## Math

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/7/76/Inner-product-angle.svg/320px-Inner-product-angle.svg.png" height="200">

- 📖 [PBRT Chapter 2 Geometry and Transformations - (2018) *Matt Pharr, Wenzel Jakob, Greg Humphreys, and Morgan Kaufmann*](http://www.pbr-book.org/3ed-2018/Geometry_and_Transformations.html)
- 📖 [PBRT Chapter 3 Shapes - (2018) *Matt Pharr, Wenzel Jakob, Greg Humphreys, and Morgan Kaufmann*](http://www.pbr-book.org/3ed-2018/Shapes.html)
- 📖 [Immersive Math - Linear Algebra - (2015) *J. Ström, K. Åström, and T. Akenine-Möller*](http://immersivemath.com/ila/index.html)
- 📺 [Linear Algebra - *Khan Academy*](https://www.khanacademy.org/math/linear-algebra)

## Ray Casting

<img src="https://upload.wikimedia.org/wikipedia/commons/6/6c/Ray_triangle.png" height="150"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/2a/Example_of_bounding_volume_hierarchy.svg/320px-Example_of_bounding_volume_hierarchy.svg.png" height="150">

- 📖 [Ray-Triangle Intersection: Geometric Solution - *Scratchapixel*](https://www.scratchapixel.com/lessons/3d-basic-rendering/ray-tracing-rendering-a-triangle/ray-triangle-intersection-geometric-solution)
- 📖 [Realtime Rendering Object/Object Intersection Page - (2019) *Eric Haines*](http://www.realtimerendering.com/intersections.html)
- 📖 [ERIT: A Collection of Efficient and Reliable Intersection Tests - (1998) *Martin Held*](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.49.9172&rep=rep1&type=pdf)
- 📖 [Introduction to Acceleration Structures - *Scratchapixel*](https://www.scratchapixel.com/lessons/advanced-rendering/introduction-acceleration-structure/bounding-volume)
- 📖 [PBRT Chater 4 Primitives and Intersection Acceleration - (2018) *Matt Pharr, Wenzel Jakob, Greg Humphreys, and Morgan Kaufmann*](http://www.pbr-book.org/3ed-2018/Primitives_and_Intersection_Acceleration.html)
- 📖 [Dynamic BVH - (2019) *Erin Catto*](http://box2d.org/files/GDC2019/ErinCatto_DynamicBVH_Full.pdf)
- 📺 [How to Make 3D Fractals](https://www.youtube.com/watch?v=svLzmFuSBhk)

## BxDF

<img src="https://upload.wikimedia.org/wikipedia/en/thumb/d/d8/BSDF05_800.png/179px-BSDF05_800.png" height="200">

- 📖 [PBRT Chapter 5.6 Surface Reflection - (2018) *Matt Pharr, Wenzel Jakob, Greg Humphreys, and Morgan Kaufmann*](http://www.pbr-book.org/3ed-2018/Color_and_Radiometry/Surface_Reflection.html)
- 📖 [PBRT Chapter 8 Reflection Models - (2018) *Matt Pharr, Wenzel Jakob, Greg Humphreys, and Morgan Kaufmann*](http://www.pbr-book.org/3ed-2018/Reflection_Models.html)
- 📖 [PBRT Chapter 9 Materials - (2018) *Matt Pharr, Wenzel Jakob, Greg Humphreys, and Morgan Kaufmann*](http://www.pbr-book.org/3ed-2018/Materials.html)
- 📖 [PBRT Chapter 11 Volume Scattering - (2018) *Matt Pharr, Wenzel Jakob, Greg Humphreys, and Morgan Kaufmann*](http://www.pbr-book.org/3ed-2018/Volume_Scattering.html)
- 📺 [Geometric Optics Playlist - (2013) *Doc Schuster*](https://www.youtube.com/playlist?list=PLLUpvzaZLf3IB4GEhaCg7L3ioiLkHLk7Q)
- 📖 [Physically Based Sky, Atmosphere, and Cloud Rendering in Frostbite - (2016) *Sebastien Hillaire*](https://media.contentapi.ea.com/content/dam/eacom/frostbite/files/s2016-pbs-frostbite-sky-clouds-new.pdf)
- 📖 [Revisiting Physically Based Shading in ImageWorks - (2017) *Christopher Kulla & Alejandro Conty*](https://blog.selfshadow.com/publications/s2017-shading-course/imageworks/s2017_pbs_imageworks_slides.pdf)
- 📖 [A Multifaceted Explanation Part 1 - (2018) *Stephen Hill*](https://blog.selfshadow.com/2018/05/13/multi-faceted-part-1/)
  - 📖 [A Multifaceted Explanation Part 2 - (2018) *Stephen Hill*](https://blog.selfshadow.com/2018/06/04/multi-faceted-part-2/)
  - 📖 [A Multifaceted Explanation Part 3 - (2018) *Stephen Hill*](https://blog.selfshadow.com/2018/08/05/multi-faceted-part-3/)
  
## Sampling Methods

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/a4/Hammersley_set_2D.svg/289px-Hammersley_set_2D.svg.png" height="200">

- 📖 [PBRT Chapter 7 - (2018) *Matt Pharr, Wenzel Jakob, Greg Humphreys, and Morgan Kaufmann*](http://www.pbr-book.org/3ed-2018/Sampling_and_Reconstruction.html)
- 📖 [Generating Random Points in a Sphere - (2018) *Karthik Karanth*](https://karthikkaranth.me/blog/generating-random-points-in-a-sphere/)
- 📖 [Robust Monte Carlo Methods Chapters 2, 9, & 11 - (1998) *Eric Veach*](https://graphics.stanford.edu/papers/veach_thesis/)
- 📖 [Flavors of Sampling in Ray Tracing  - (2018) *Peter Shirley*](http://psgraphics.blogspot.com/2018/10/flavors-of-sampling-in-ray-tracing.html)
- 📺 [Continuous Multiple Importance Sampling - SIGGRAPH 2020 - (2020) *Rex West, Iliyan Georgiev , Adrien Gruson , Toshiya Hachisuka*](https://youtu.be/dxFSwplfdpk)
- 📖 [Position-Free Monte Carlo Simulation for Arbitrary Layered BSDFs - (2018) *Yu Guo, Miloš Hašan, Shuang Zhao*](https://shuangz.com/projects/layered-sa18/)
- 📖 [Monte Carlo Integration - *Anders Lindqvist*](https://www.breakin.se/mc-intro/)
- 📖 [Monte Carlo Integration Explanation in 1D - (2018) *Alan Wolfe*](https://blog.demofox.org/2018/06/12/monte-carlo-integration-explanation-in-1d/)
- 📖 [Importance Sampling techniques for GGX with Smith Masking-Shadowing Part 1 - (2018) *Joe Schutte*](https://schuttejoe.github.io/post/ggximportancesamplingpart2/)
  - 📖 [Importance Sampling techniques for GGX with Smith Masking-Shadowing Part 2 - (2018) *Joe Schutte*](https://schuttejoe.github.io/post/ggximportancesamplingpart2/)
- 📖 [Double Hierarchies for Directional Importance Sampling in Monte Carlo Rendering - (2018) *Norbert Bus and Tamy Boubekeur*](http://www.jcgt.org/published/0006/03/02/)
- 📖 [Importance Sampling of Many Lights with Adaptive Tree Splitting - (2018) *Alejandro Conty and Christopher Kulla*](https://docs.google.com/viewer?a=v&pid=sites&srcid=ZGVmYXVsdGRvbWFpbnxja3VsbGF8Z3g6NWM0NmU2YWVlNjE3ODk1Yw)
- 📖 [Monte Carlo Methods for Volumetric Light Transport Simulation - (2018) *Jan Novák, Iliyan Georgiev, Johannes Hanika, and Wojciech Jarosz*](http://iliyan.com/publications/VolumeSTAR)

## Denoising, Filtering, and Reconstruction

<img src="https://upload.wikimedia.org/wikipedia/commons/f/f4/Noise_salt_and_pepper.png" height="200">

- 📺 [RTX Coffee Break: Ray Tracing and Denoising - (2018) *Edward Lu*](https://news.developer.nvidia.com/rtx-coffee-break-ray-tracing-and-denoising/)
- 📺 [RTX Coffee Break: Ray Traced Reflections and Denoising - (2018) *Edward Lu*](https://news.developer.nvidia.com/rtx-coffee-break-ray-traced-reflections-and-denoising-952-minutes/)
- 📖 [Spatiotemporal Variance-Guided Filtering: Real-Time Reconstruction for Path-Traced Global Illumination - (2017) *Christoph Schied, Anton Kaplanyan, Chris Wyman, Anjul Patney, Chakravarty R. Alla Chaitanya, John Burgess, Shiqiu Liu, Carsten Dachsbacher, Aaron Lefohn, Marco Salvi*](http://cg.ivd.kit.edu/svgf.php)
- 📖 [Multidimensional Adaptive Sampling and Reconstruction for Ray Tracing - (2008) *Toshiya Hachisuka, Wojciech Jarosz, Richard Peter Weistroffer, Kevin Dale, Greg Humphreys, Matthias Zwicker, and Henrik Wann Jensen*](http://graphics.ucsd.edu/~henrik/papers/multidimensional_adaptive_sampling/)

## Realtime

- 📖 [Real-Time Rendering Chapter - (2018) *Tomas Akenine-Möller, Eric Haines, Naty Hoffman, Angelo Pesce, Michał Iwanicki, and Sébastien Hillaire*](http://www.realtimerendering.com/Real-Time_Rendering_4th-Real-Time_Ray_Tracing.pdf)
- 📺 [Real-Time Raytracing for Interactive Global Illumination Workflows in Frostbite / Shiny Pixels and Beyond: Real-Time Raytracing at SEED - (2018) *Sébastien Hillaire, Johan Andersson, and Colin Barré-Brisebois*](https://youtu.be/rhlGBCSv02M)
- 📖 [Real-Time Ray Tracing of Correct* Soft Shadows - (2018) *Stephen Hill and Morgan McGuire*](http://advances.realtimerendering.com/s2018/s2018_real_time_correct_soft_shadows.pdf)
- 📺 [Stochastic All the Things: Raytracing in Hybrid Real-Time Rendering - (2018) *Tomasz Stachowiak*](https://www.ea.com/seed/news/seed-dd18-presentation-slides-raytracing)
- 📖 [Adopting Lessons From Offline Ray-Tracing to Real-Time Ray-Tracing for Practical Pipelines - (2018) *Matt Pharr*](http://advances.realtimerendering.com/s2018/Pharr%20-%20Advances%20in%20RTR%20-%20Real-time%20Ray%20Tracing.pdf)
- 📖 [Game Ray Tracing: State-of-the-Art and Open Problems - (2018) *Colin Barré Brisebois*](https://www.ea.com/seed/news/hpg-2018-keynote)
- 💾 [Sol-R, an Open-Source CUDA/OpenCL Speed Of Light Ray-tracer](https://github.com/favreau/Sol-R)

## Reference Scenes

<img src="https://upload.wikimedia.org/wikipedia/commons/2/24/Cornell_box.png" height="200"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/43/Stanford_Bunny.stl/320px-Stanford_Bunny.stl.png" height="200">

- 💾 [McGuire Computer Graphics Archive](http://casual-effects.com/data/index.html)
- 💾 [Benedikt Bitterli](https://benedikt-bitterli.me/resources/)
- 💾 [PBRT Scenes v3](https://www.pbrt.org/scenes-v3.html)
- 💾 [ORCA: Open Research Content Archive](https://developer.nvidia.com/orca)
- 💾 [Disney Data Sets](https://www.technology.disneyanimation.com/collaboration-through-sharing)

## News

- 📖 [Graphics Programming Weekly - *Jendrik Illner*](https://www.jendrikillner.com/post/)

## API's

- [Vulkan Ray Tracing](https://www.khronos.org/registry/vulkan/specs/1.2-extensions/man/html/VK_KHR_ray_tracing.html)
- [Nvidia RTX](https://developer.nvidia.com/rtx)
- [Microsoft DirectX Raytracing (DXR)](https://blogs.msdn.microsoft.com/directx/2018/03/19/announcing-microsoft-directx-raytracing/)
- [Nvidia OptiX](https://developer.nvidia.com/optix)
- [AMD Radeon-Rays](https://gpuopen.com/radeon-rays/)
- [Intel Embree](http://embree.github.io/)

### Vulkan Ray Tracing

- 📖 [Ray Tracing In Vulkan - (2020) *Khronos*](https://www.khronos.org/blog/ray-tracing-in-vulkan)
- 📖 [Vulkan Ray Tracing Tutorials - (2020) *Nvidia*](https://github.com/nvpro-samples/vk_raytracing_tutorial_KHR)

### Nvidia RTX

- 📖 [NVIDIA Vulkan Ray Tracing Tutorial - (2018) *NVidia*](https://developer.nvidia.com/rtx/raytracing/vkray)
- 📖 [Introduction to Real-Time Ray Tracing with Vulkan - (2018) *Nuno Subtil*](https://devblogs.nvidia.com/vulkan-raytracing/)
- 📖 [Vulkan Raytracing Tutorials - (2018) *iOrange*](https://iorange.github.io/p02/TeapotAndBunny.html)
- 📺 [Video Series: Practical Real-Time Ray Tracing With RTX - (2018) *Nvidia*](https://devblogs.nvidia.com/practical-real-time-ray-tracing-rtx/)
- 📖 [Effectively Integrating RTX Ray Tracing into a Real-Time Rendering Engine - (2018) *Juha Sjoholm*](https://devblogs.nvidia.com/effectively-integrating-rtx-ray-tracing-real-time-rendering-engine/)

### Microsoft DirectX Raytracing (DXR)

- 📺📖 [Introducion to DirectX Raytracing - (2018) *Chris Wyman, Shawn Hargreaves, Peter Shirley, Colin Barré-Brisebois*](http://intro-to-dxr.cwyman.org/)
- 📖 [DX12 Ray Tracing Tutorials - (2018) *Martin-Karl Lefrançois and Pascal Gautron*](https://news.developer.nvidia.com/dx12-raytracing-tutorials/)
- 💾 [DXRPathTracer](https://github.com/TheRealMJP/DXRPathTracer)
- 📺 [Real-Time Ray Tracing for Interactive Global Illumination Workflows in Frostbite - (2018) *Sebastien Hillaire, Charles de Rousiers, Diede Apers and Petter Edblom*](https://devblogs.nvidia.com/video-real-time-ray-tracing-workflows-frostbite/)

### Nvidia OptiX

- 📖 [Introduction to OptiX - (2017) *Nvidia*](http://on-demand.gputechconf.com/gtc/2017/presentation/s7455-martin-stich-optix.pdf)
- 📖 [OptiX QuickStart - *Nvidia*](https://docs.nvidia.com/gameworks/content/gameworkslibrary/optix/optix_quickstart.htm)
- 📖 [Ray Tracing The Next Week in OptiX - (2018) *João Vítor Silva*](https://joaovbs96.github.io/optix/2018/12/24/next-week.html)
- 💾 [optix_advanced_samples - (2018) *Nvidia*](https://github.com/nvpro-samples/optix_advanced_samples)
- 📺 [GPU Ray Tracing for Film and Design: High Performance Ray Tracing with OptiX - (2018) *Oliver Klehm*](http://on-demand.gputechconf.com/siggraph/2018/video/sig1812-2-oliver-klehm-high-performance-optix.html)

## Applications

### Embree

| Property | Value |
| --- | --- |
| Link | 💾 [Embree](https://github.com/embree/embree) |
| About | Embree ray tracing kernels repository |
| Language | C++ |
| OS | Windows (32-bit and 64-bit), Linux (64-bit), and macOS (64-bit) |
| Compiler | Intel® Compiler, GCC, Clang, and the Microsoft Compiler |
| Linux Dependencies | cmake tbb-devel glfw-devel |
| Windows dependencies | CMake |
| General dependencies | at least an x86 CPU with support for SSE2 <br> or an Apple M1 CPU |
| Licence | Apache-2.0 |

### GLSL-PathTracer

| Property | Value |
| --- | --- |
| Link | 💾 [GLSL-PathTracer](https://github.com/knightcrawler25/GLSL-PathTracer) |
| About | A physically based path tracer that runs in a GLSL fragment shader |
| Language | C++, GLSL (OpenGL Shading Language) |
| OS | Linux, Windows |
| Linux Dependencies | libdsl2 |
| Windows dependencies | VS |
| General dependencies | |
| Licence | MIT |

### Sprout

| Property | Value |
| --- | --- |
| Link | 💾 [Sprout](https://github.com/bolero-MURAKAMI/Sprout) |
| About | C++11/14 constexpr based Containers, Algorithms, Random numbers, Parsing, Ray tracing, Synthesizer, and others |
| Language | C++ |
| OS | Linux |
| Linux Dependencies | GCC, C++11/14/17 |
| | Clang, C++11/14/17 |
| General dependencies |  |
| Licence | BSL-1.0 |

tryout

### NanoRT

| Property | Value |
| --- | --- |
| Link | 💾 [nanort](https://github.com/lighttransport/nanort) |
| About | NanoRT, single header only modern ray tracing kernel |
| Language | C++ |
| OS | MacOSX, Linux, Windows, iOS, Android, ARM, x86, SPARC, (maybe) MIPS, (will be) RISC-V, etc. |
| Licence | MIT |

tryout

### LuxCore

| Property | Value |
| --- | --- |
| Link | 💾 [LuxCore](https://github.com/LuxCoreRender/LuxCore) |
| About | LuxCoreRender is a physically correct, unbiased rendering engine |
| Language | C++ |
| Windows dependencies | Visual Studio 2017 |
| Licence | Apache-2.0 |

### OSPRay

| Property | Value |
| --- | --- |
| Link | 💾 [Intel OSPRay](https://www.ospray.org/) |
| About | An Open, Scalable, Portable, Ray Tracing Based Rendering Engine for High-Fidelity Visualization  |
| Language | C, C++ |
| OS | Linux, Mac OS X, and Windows |
| Linux Dependencies | cmake, tbb-devel |
| Windows dependencies |  CMake, TBB, ISPC (for your Visual Studio version), Embree |
| General dependencies | Intel oneAPI Rendering Toolkit common library <br> Intel Embree <br> Intel ISPC (Implicit SPMD Program Compiler) <br> Intel Open VKL |
| Licence | Apache-2.0 |

### PlotOptiX

| Property | Value |
| --- | --- |
| Link | 💾 [PlotOptiX](https://github.com/rnd-team-dev/plotoptix) |
| About | Data visualisation in Python based on OptiX 7.2 ray tracing framework.  |
| Language | Python |
| OS | Windows 10, Ubuntu 18.04, CentOS 7 |
| Linux Dependencies | Mono Common Language Runtime >= 5.2 <br> pythonnet >= 2.5.1 <br> FFmpeg >= 4.1 |
| Windows dependencies | .NET Framework >= 4.6.1  |
| General dependencies | Python 3 64-bit <br> NVIDIA OptiX 7.2 |
| Licence | PlotOptiX is free for non-commercial use |

### Visionaray

| Property | Value |
| --- | --- |
| Link | 💾 [Visionaray](https://github.com/szellmann/visionaray) |
| About | A C++-based, cross platform ray tracing library   |
| Language | C++ |
| OS | Linux, Mac OS X, and Windows |
| Linux Dependencies | C++11 compiler (tested with g++-7.4.0 on Ubuntu 18.04 x86_64 |
| Mac OS dependencies | clang-900.0.39.2 |
| Windows dependencies | Microsoft Visual Studio 2015 VC14 for x64 |
| General dependencies | CMake version 3.1.3 or newer <br> OpenGL <br>  GLEW <br> Boost <br> GLUT  |
| Licence | MIT |

tryout

### SORT

| Property | Value |
| --- | --- |
| Link | 💾 [SORT](https://github.com/JiayinCao/SORT) |
| About | Simple Open-source Ray Tracing |
| Language | C++, Python |
| OS | Windows, Ubuntu, MacOS |
| Licence | GPL-3.0 License  |

### c-ray

| Property | Value |
| --- | --- |
| Link | 💾 [c-ray](https://github.com/vkoskiv/c-ray) |
| About | C-ray is a research oriented, hackable, offline CPU rendering engine built for learning. |
| Language | C |
| OS |  |
| Linux Dependencies |  |
| Windows dependencies |  |
| General dependencies |  |
| Licence | MIT |


### voxel-cone-tracing

| Property | Value |
| --- | --- |
| Link | 💾 [voxel-cone-tracing](https://github.com/Friduric/voxel-cone-tracing) |
| About | A real-time global illumination implementation using voxel cone tracing. Implemented in C++ and GLSL.  |
| Language | C, C++ |
| General dependencies | CMake OpenGL 4.4 |
| Licence | MIT |
| Comment | last submit 5 y old |

### minpt

| Property | Value |
| --- | --- |
| Link | 💾 [minpt](https://github.com/hi2p-perim/minpt) |
| About |A path tracer in 300 lines of C++   |
| Language | C++ |
| OS |  |
| Linux Dependencies |  |
| Windows dependencies |  |
| General dependencies | OpenMP  |
| Licence | ~GPL (?) |
| Comment | last submit 2 y old |


### lightmetrica-v3

| Property | Value |
| --- | --- |
| Link | 💾 [lightmetrica-v3](https://github.com/lightmetrica/lightmetrica-v3) |
| About | A research-oriented renderer  |
| Language | C++ Python |
| OS | Windows, Mac OS X, Linux |
| Linux Dependencies |  |
| Windows dependencies |  |
| General dependencies |  |
| Licence |  |
| Comment | [Extensive documentation](https://lightmetrica.github.io/lightmetrica-v3-doc/build.html) |

### BVH

| Property | Value |
| --- | --- |
| Link | 💾 [bvh](https://github.com/madmann91/bvh) |
| About | This is a modern C++17 header-only BVH library optimized for ray-tracing. |
| Language | C++ |
| OS |  |
| General dependencies | OpenMP |
| Licence | MIT |

### DiligentEngine

| Property | Value |
| --- | --- |
| Link | 💾 [DiligentEngine](https://github.com/DiligentGraphics/DiligentEngine) |
| About | A modern cross-platform low-level graphics library and rendering framework  |
| Language | C++ |
| OS |  |
| Linux Dependencies |  |
| Windows dependencies |  |
| General dependencies | take full advantage of Direct3D12, Vulkan and Metal, while supporting older platforms via Direct3D11, OpenGL and OpenGLES |
| Licence | Apache 2.0 |

### The-Forge

| Property | Value |
| --- | --- |
| Link | 💾 [The-Forge](https://github.com/ConfettiFX/The-Forge) |
| About | The Forge is a cross-platform rendering framework |
| Language |  |
| OS |  |
| Linux Dependencies |  |
| Windows dependencies |  |
| General dependencies |  |
| Licence | Apache 2.0  |



### Template

| Property | Value |
| --- | --- |
| Link | 💾 []() |
| About |  |
| Language |  |
| OS |  |
| Linux Dependencies |  |
| Windows dependencies |  |
| General dependencies |  |
| Licence |  |



