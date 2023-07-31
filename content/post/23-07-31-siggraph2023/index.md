---
title: Des contributions françaises à SIGGRAPH 2023
date: 2023-07-31
draft: false
authors:
  - Étienne Peillard
---

## A Sparse Non-parametric BRDF Model
*Tanaboon Tongbuasirilai, Jonas Unger (Linkoping University), Christine Guillemot (INRIA), Ehsan Miandji (Linkoping University)*

{{< figure src="Tongbuasirilai2023.png" caption="An overview of the proposed framework for learning accurate representations and sparse data-driven BRDF models through analysis of the space of BRDFs. The BRDF dictionary ensemble is trained once and can accurately represent a wide range of previously unseen materials.">}}

This paper presents a novel sparse non-parametric BRDF model derived using a machine learning approach to represent the space of possible BRDFs using a set of multidimensional sub-spaces, or dictionaries. By training the dictionaries under a sparsity constraint, the model guarantees high quality representations with minimal storage requirements and an inherent clustering of the BDRF-space. The model can be trained once and then reused to represent a wide variety of measured BRDFs. Moreover, the proposed method is flexible to incorporate new unobserved data sets, parameterizations, and transformations. In addition, we show that any two, or more, BRDFs can be smoothly interpolated in the coefficient space of the model rather than the significantly higher-dimensional BRDF space. The proposed sparse BRDF model is evaluated using the MERL, DTU and RGL-EPFL BRDF databases. Experimental results show that the proposed approach results in about 9.75dB higher SNR on average for rendered images as compared to current state-of-the-art models.

[*Full paper*](https://hal.science/hal-03654734/)

## VideoDoodles: Hand-drawn Animations on Videos With Scene-aware Canvases
*Emilie Yu (Centre Inria d'Universite Cote d'Azur), Kevin Matzen, Cuong Nguyen, Oliver Wang, Rubaiat Habib Kazi (Adobe), Adrien Bousseau (Centre Inria d'Universite Cote d'Azur and TU Delft)*

{{< figure src="Yu2023.png" caption="Video doodles combine hand-drawn animations with video footage. Our interactive system eases the creation of this mixed media art by letting users place planar canvases in the scene which are then tracked in 3D. In this example, the inserted rainbow bridge exhibits correct perspective and occlusions, and the character’s face and arms follow the tram as it runs towards the camera.">}}

We present an interactive system to ease the creation of so-called video doodles – videos on which artists insert hand-drawn animations for entertainment or educational purposes. Video doodles are challenging to create because to be convincing, the inserted drawings must appear as if they were part of the captured scene. In particular, the drawings should undergo tracking, perspective deformations and occlusions as they move with respect to the camera and to other objects in the scene – visual effects that are difficult to reproduce with existing 2D video editing software. Our system supports these effects by relying on planar canvases that users position in a 3D scene reconstructed from the video. Furthermore, we present a custom tracking algorithm that allows users to anchor canvases to static or dynamic objects in the scene, such that the canvases move and rotate to follow the position and direction of these objects. When testing our system, novices could create a variety of short animated clips in a dozen of minutes, while professionals praised its speed and ease of use compared to existing tools.

{{< video src="https://em-yu.github.io/media/figures/VideoDoodles/RESULTS_ours.mp4" controls="yes" >}}

[*Full paper*](https://em-yu.github.io/research/videodoodles/)

## Large-scale Terrain Authoring Through Interactive Erosion Simulation
*Hugo Schott, Axel Paris, Lucie Fournier, Eric Guerin, Eric Galin (Univ Lyon / INSA Lyon / CNRS / UCBL / LIRIS / UMR5205)*

{{< figure src="Schott2023.png" caption="Given an input uplift field, we automatically generate the large-scale terrain elevation by simulating stream power erosion using a parallel drainage area algorithm inlined in the simulation. The user may define the uplift field, providing ridge and river networks, or using inverse procedural modeling by computing the uplift from an input digital elevation model.">}}

Large-scale terrains are essential in the definition of virtual worlds. Given the diversity of landforms and the geomorphological complexity, there is a need for authoring techniques offering hydrological consistency without sacrificing user control. In this paper, we bridge the gap between large-scale erosion simulation and authoring into an efficient framework. We set aside modeling in the elevation domain in favour of the uplift domain, and compute emerging reliefs by simulating the stream power erosion. Our simulation relies on a fast yet accurate approximation of drainage area and flow routing to compute the erosion interactively, which allows for incremental authoring. Our model provides landscape artists with tools for shaping mountain ranges and valleys, such as copy-and-paste operations; warping for imitating folds and faults; point and curve elevation constraints to precisely sculpt ridges or carve river networks. It also lends itself to inverse procedural modeling by reconstructing the uplift from an input digital elevation model and allows hydrologically consistent blending between terrain patches. 

{{< youtube id=gCP7jzcPLyQ >}}

[*Full paper*](https://hal.archives-ouvertes.fr/hal-04049125/)

## Forming Terrains by Glacial Erosion
*Guillaume Cordonnier (Inria and Universite Cote d'Azur), Guillaume Jouvet (University of Lausanne), Adrien Peytavie (Univ Lyon / INSA Lyon / CNRS / UCBL / LIRIS / UMR5205), Jean Braun (Helmholtz Centre Potsdam and University of Potsdam), Marie-Paule Cani (Ecole Polytechnique), Bedrich Benes (Purdue University), Eric Galin, Eric Guerin (Univ Lyon / INSA Lyon / CNRS / UCBL / LIRIS / UMR5205), James Gain (University of Cape Town)*

{{< figure src="Cordonnier2023.png" caption="A landscape carved by our simulated glacier. Specific landforms are (1) U-shaped valleys, (2) hanging valleys, (3) a glacial cirque overhung by arêtes and horns, (4) a pass, and (5) high–altitude lakes.">}}

We introduce the first solution for simulating the formation and evolution of glaciers, together with their attendant erosive effects, for periods covering the combination of glacial and inter-glacial cycles. Our efficient solution includes both a fast yet accurate deep learning-based estimation of high-order ice flows and a new, multi-scale advection scheme enabling us to account for the distinct time scales at which glaciers reach equilibrium compared to eroding the terrain. We combine the resulting glacial erosion model with finer-scale erosive phenomena to account for the transport of debris flowing from cliffs. This enables us to model the formation of terrain shapes not previously adequately modeled in Computer Graphics, ranging from U-shaped and hanging valleys to fjords and glacial lakes. 

{{< youtube id=xfk_J4VhdWA >}}

[*Full paper*](https://hal.archives-ouvertes.fr/hal-04090644/)

## ConTesse: Accurate Occluding Contours for Subdivision Surfaces
*Chenxi Liu (University of British Columbia), Pierre Benard (University of Bordeaux / CNRS / Bordeaux INP / INRIA / LaBRI), Aaron Hertzmann (Adobe Research), Shayan Hoshyari (Adobe)*

{{< figure src="Liu2023.jpg" caption="Given (a) a smooth 3D surface and a camera viewpoint, our method produces (b) a triangle mesh where the occluding contour of the mesh accurately approximates the occluding contour of the smooth surface. Standard algorithms may then be used to extract (c) the view map of occluding contours, and to (d) stylize them. (Fertility courtesy UU from AIM@SHAPE-VISIONAIR Shape Repository). ">}}

This paper proposes a method for computing the visible occluding contours of subdivision surfaces. The paper first introduces new theory for contour visibility of smooth surfaces. Necessary and sufficient conditions are introduced for when a sampled occluding contour is valid, that is, when it may be assigned consistent visibility. Previous methods do not guarantee these conditions, which helps explain why smooth contour visibility has been such a challenging problem in the past. The paper then proposes an algorithm that, given a subdivision surface, finds sampled contours satisfying these conditions, and then generates a new triangle mesh matching the given occluding contours. The contours of the output triangle mesh may then be rendered with standard non-photorealistic rendering algorithms, using the mesh for visibility computation. The method can be applied to any triangle mesh, by treating it as the base mesh of a subdivision surface. 

[*Full paper*](https://dgp.toronto.edu/~hertzman/contesse/contesse_arxiv.pdf)

## Polynomial 2D Green Coordinates for Polygonal Cages
*Elie Michel, Jean-Marc Thiery (Adobe Research)*

{{< figure src="Michel2023.png" caption="Top row: (a) input image and an embedding polygonal cage; (b-d) deformations obtained using Mean-Value coordinates, Cubic Mean-Value coordinates, and Green coordinates; (e) our conformal deformations obtained with cubic curves. Bottom row: more resuls of our approach, using polynomial curves of various orders (from 1 to 7).">}}

Cage coordinates are a powerful means to define 2D deformation fields from sparse control points. We introduce Conformal polynomial Coordinates for closed polyhedral cages, enabling segments to be transformed into polynomial curves of any order. Extending classical 2D Green coordinates, our coordinates result in conformal harmonic deformations that are cage-aware. We demonstrate the usefulness of our technique on a variety of 2D deformation scenarios where curves allow artists to perform intuitive deformations with few input parameters. Our method combines the texture preservation property of conformal deformations together with the expressiveness offered by Bezier controls.

[*Full paper*](https://portfolio.exppad.com/documents/2023__Michel__PolynomialGreenCoords.pdf)

## Orientable Dense Cyclic Infill for Anisotropic Appearance Fabrication
*Xavier Chermain, Cedric Zanni, Jonas MartÃ­nez, Pierre-Alexandre Hugron, Sylvain Lefebvre (Universite de Lorraine / CNRS / Inria)*

{{< figure src="Chermain2023.png" caption="We develop an efficient algorithm that produces an orientable dense cyclic infill by aligning a field of periodic functions, contouring it to obtain cycles, and connecting all cycles into one. We leverage this algorithm to print anisotropic appearances using fused filament fabrication. Left: the shape with purple boundaries is infilled with a cycle. The cycle’s directions have four modes: parallel to the boundary (red area), orthogonal to the boundary (blue area), smoothest lines (yellow area), and constrained lines (color gradient area). Our algorithm is very flexible, allowing directions to be constrained everywhere (areas with a color gradient in the logo) or only within the vicinity of the boundary (blue, red, and yellow areas). Alignment with boundaries can also be constrained, as in this example. The grey cycle is the output of our algorithm (curve interspace objective: 2.5 mm). Right: Printed cycle with interspace set to 0.4 mm. The trajectory’s directions determine the appearance, as extruded filaments exhibit anisotropic roughness.">}}

We present a method to 3D print surfaces exhibiting a prescribed varying field of anisotropic appearance using only standard fused filament fabrication printers. This enables the fabrication of patterns triggering reflections similar to that of brushed metal with direct control over the directionality of the reflections. Our key insight, on which we ground the method, is that the direction of the deposition paths leads to a certain degree of surface roughness, which yields a visual anisotropic appearance. Therefore, generating dense cyclic infills aligned with a line field allows us to grade the anisotropic appearance of the printed surface. To achieve this, we introduce a highly parallelizable algorithm for optimizing oriented, cyclic paths. Our algorithm outperforms existing approaches regarding efficiency, robustness, and result quality. We demonstrate the effectiveness of our technique in conveying an anisotropic appearance on several challenging test cases, ranging from patterns to photographs reinterpreted as anisotropic appearances.

{{< youtube id=aUDzZrlRnNU >}}

[*Full paper*](https://xavierchermain.github.io/data/pdf/Chermain2023Orientable.pdf)

## Complex Wrinkle Field Evolution
*Zhen Chen (The University of Texas at Austin), Danny Kaufman (Adobe Research), Melina Skouras (Univ. Grenoble Alpes / Inria / CNRS), Etienne Vouga (The University of Texas at Austin)*

{{< figure src="Chen2023.webp" caption="We propose Complex Wrinkle Fields (CWF s), a new discrete wrinkle model that enables the resolution of highly detailed wrinkle patterns on coarse base-mesh geometry. The CWF representation consists of a positive number a per vertex encoding the wrinkle amplitude, a one-form ω per edge to model wrinkle frequency, and a complex number ˜z per vertex to represent wrinkle phase, coupled via a weak variational consistency condition ensuring that ˜z can capture singularities while also being as compatible with ω as possible (§ 3.1). We equip the CWF representation with a novel temporal interpolation algorithm (§ 4) and a spatial upsampling method (§ 5) that together allow for smooth interpolation between wrinkle patterns represented on surfaces by CWF s (leftmost and rightmost column), and base-mesh-independent rendering of arbitrarily high-resolution wrinkle patterns. Together these contributions make it possible to smoothly evolve wrinkle patterns between two prescribed keyframes (middle columns) with automatic merging, splitting, and reconnection of wrinkles as necessary via smooth sliding of singularities across the surface (zoomed-in figures in middle columns). ">}}

We propose a new approach for representing wrinkles, designed to capture complex and detailed wrinkle behavior on coarse triangle meshes, called Complex Wrinkle Fields. Complex Wrinkle Fields consist of an almost-everywhere-unit complex-valued phase function over the surface; a frequency one-form; and an amplitude scalar, with a soft compatibility condition coupling the frequency and phase. We develop algorithms for interpolating between two such wrinkle fields, for visualizing them as displacements of a Loop-subdivided refinement of the base mesh, and for making smooth local edits to the wrinkle amplitude, frequency, and/or orientation. These algorithms make it possible, for the first time, to create and edit animations of wrinkles on triangle meshes that are smooth in space, evolve smoothly through time, include singularities along with their complex interactions, and that represent frequencies far finer than the surface resolution.

[*Full paper*](https://zhenchen-jay.github.io/uploads/CWF.pdf)

## Coupling Conduction, Convection and Radiative Transfer in a Single Path-Space: Application to Infrared Rendering
*Megane Bati, Stephane Blanco (Univ. Toulouse), Christophe Coustet, Vincent Eymet, Vincent Forest (Meso-Star), Richard Fournier (Univ. Toulouse), Jacques Gautrais (Univ. Toulouse and CNRS), Nicolas Mellado, Mathias Paulin (Univ. Toulouse), Benjamin Piaud (Meso-Star)*

{{< figure src="Bati2023.png" caption="We propose a Monte Carlo approach to tackle multiple physics with a single algorithm, translating their coupling into a single path-space composed of randomly chained sub-paths for each physics. Application is exemplified with heat transfer. (a) An infrared image of a steady state thermal exchanger, with temperature imposed on the left and right walls. (b) Monte Carlo paths alternate between heat-transfer modes (here conduction and radiation). (c) A huge benefit is the fast production of transient simulations, at any time, using the information gathered in (a), i.e. from only one Monte Carlo run at steady state. ">}}

In the past decades, Monte Carlo methods have shown their ability to solve PDEs, independently of the dimensionality of the integration domain and for different use-cases (e.g. light transport, geometry processing, physics simulation). Specifically, the path-space formulation of transport equations is a key ingredient to define tractable and scalable solvers, and we observe nowadays a strong interest in the definition of simulation systems based on Monte Carlo algorithms. We also observe that, when simulating combined physics (e.g. thermal rendering from a heat transfer simulation), there is a lack of coupled Monte Carlo algorithms allowing to solve all the physics at once, in the same path space, rather than combining several independent MC estimators, a combination that would make the global solver critically sensitive to the complexity of each simulation space. This brings to our proposal: a coupled, single path-space, Monte Carlo algorithm for efficient multi-physics problems solving. In this work, we combine our understanding and knowledge of Physics and Computer Graphics to demonstrate how to formulate and arrange different simulation spaces into a single path space. We define a tractable formalism for coupled heat transfer simulation using Monte Carlo, and we leverage the path-space construction to interactively compute multiple simulations with different conditions in the same scene, in terms of boundary conditions and observation time. We validate our proposal in the context of infrared rendering with different thermal simulation scenarios: e.g., room temperature simulation, visualization of heat paths within materials (detection of thermal bridges), heat diffusion capacity of thermal exchanger. We expect that our theoretical framework will foster collaboration and multidisciplinary studies. The perspectives this framework opens are detailed and we suggest a research agenda towards the resolution of coupled PDEs at the interface of Physics and Computer Graphics. 

{{< youtube id=UIjgiNymjyw >}}

[*Full paper*](https://hal.science/hal-04090428)

## Textured Mesh Quality Assessment: Large-scale Dataset and Deep Learning-based Quality Metric


## Variational Shape Reconstruction via Quadric Error Metrics


## Somigliana Coordinates: An Elasticity-derived Approach for Cage Deformation


## Constraint-based Simulation of Passive Suction Cups


## MesoGen: Designing Procedural On-surface Stranded Mesostructures


## Fluid-solid Coupling in Kinetic Two-phase Flow Simulation


## GREIL-Crowds: Crowd Simulation With Deep Reinforcement Learning and Examples


## 3D Gaussian Splatting for Real-Time Radiance Field Rendering


## PCBend: Light Up Your 3D Shapes With Foldable Circuit Boards


## Fast GPU-based Two-way Continuous Collision Handling
