---
title: Des contributions françaises à SIGGRAPH 2023
date: 2023-07-31
draft: false
authors:
  - Étienne Peillard
---

N'hésitez pas à nous signaler tout oubli.


{{% toc %}}

## Building a Virtual Weakly-compressible Wind Tunnel Testing Facility
*Chaoyang Lyu (ShanghaiTech University / SIMIT / UCAS), Kai Bai (ShanghaiTech University / AEROCAE Digital Ltd.), Yiheng Wu (ShanghaiTech University), Mathieu Desbrun (Inria and Ecole Polytechnique), Changxi Zheng (Tencent Pixel Lab and Columbia University), Xiaopei Liu (ShanghaiTech University)*

{{< figure src="windTunnel2023.jpeg" >}}


Virtual wind tunnel testing is a key ingredient in the engineering design process for the automotive and aeronautical industries as well as for urban planning: through visualization and analysis of the simulation data, it helps optimize lift and drag coefficients, increase peak speed, detect high pressure zones, and reduce wind noise at low cost prior to manufacturing. In this paper, we develop an efficient and accurate virtual wind tunnel system based on recent contributions from both computer graphics and computational fluid dynamics in high-performance kinetic solvers. Running on one or multiple GPUs, our massively-parallel lattice Boltzmann model meets industry standards for accuracy and consistency while exceeding current mainstream industrial solutions in terms of efficiency Ð especially for unsteady turbulent flow simulation at very high Reynolds number (on the order of 10^7) -- due to key contributions in improved collision modeling and boundary treatment, automatic construction of multiresolution grids for complex models, as well as performance optimization. We demonstrate the efficacy and reliability of our virtual wind tunnel testing facility through comparisons of our results to multiple benchmark tests, showing an increase in both accuracy and efficiency compared to state-of-the-art industrial solutions. We also illustrate the fine turbulence structures that our system can capture, indicating the relevance of our solver for both VFX and industrial product design.

{{< video src="http://www.geometry.caltech.edu/Movies/LBWD+23.mp4" controls="yes" >}}



## Patternshop: Editing Point Patterns by Image Manipulation
*Xingchang Huang (Max Planck Institute for Informatics), Tobias Ritschel (University College London), Hans-Peter Seidel (Max Planck Institute for Informatics), Pooran Memari (LIX-Inria), Gurprit Singh (Max Planck Institute for Informatics)*

{{< figure src="Huang2023.png" caption="Our framework facilitate point pattern design by representing both density and correlation as a three-channel raster image (a). These images can be edited (c) in terms of their density or correlation using off-the-shelf image manipulation software. The resulting point patterns are shown before (b) and after the edits (d). Please see the accompanied supplemental material for vector graphic images.">}}

Point patterns are characterized by their density and correlation. While spatial variation of density is well-understood, analysis and synthesis of spatially-varying correlation is an open challenge. No tools are available to intuitively edit such point patterns, primarily due to the lack of a compact representation for spatially varying correlation. We propose a low-dimensional perceptual embedding for point correlations. This embedding can map point patterns to common three-channel raster images, enabling manipulation with off-the-shelf image editing software. To synthesize back point patterns, we propose a novel edge-aware objective that carefully handles sharp variations in density and correlation. The resulting framework allows intuitive and backward-compatible manipulation of point patterns, such as recoloring, relighting to even texture synthesis that have not been available to 2D point pattern design before. Effectiveness of our approach is tested in several user experiments. Code is available at https://github.com/xchhuang/patternshop.

[*Page projet*](https://xchhuang.github.io/patternshop/)

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
*Yana Nehme, Johanna Delanoy, Florent Dupont, Jean-Philippe Farrugia (Univ Lyon, UCBL, CNRS, INSA Lyon, LIRIS, UMR5205), Patrick Le Callet (Nantes Universite, Ecole Centrale Nantes, CNRS, LS2N, UMR 6004), Guillaume Lavoue (Univ Lyon, Centrale Lyon, CNRS, INSA Lyon, UCBL, LIRIS, UMR5205, ENISE)*

{{< figure src="Nehme2023.png" caption="(a) Geometry and color spatial information and (b) visual attention complexity for the selected source models. ">}}

Over the past decade, 3D graphics have become highly detailed to mimic the real world, exploding their size and complexity. Certain applications and device constraints necessitate their simplification and/or lossy compression, which can degrade their visual quality. Thus, to ensure the best Quality of Experience (QoE), it is important to evaluate the visual quality to accurately drive the compression and find the right compromise between visual quality and data size. In this work, we focus on subjective and objective quality assessment of textured 3D meshes. We first establish a large-scale dataset, which includes 55 source models quantitatively characterized in terms of geometric, color, and semantic complexity, and corrupted by combinations of 5 types of compression-based distortions applied on the geometry, texture mapping and texture image of the meshes. This dataset contains over 343k distorted stimuli. We propose an approach to select a challenging subset of 3000 stimuli for which we collected 148929 quality judgments from over 4500 participants in a large-scale crowdsourced subjective experiment. Leveraging our subject-rated dataset, a learning-based quality metric for 3D graphics was proposed. Our metric demonstrates state-of-the-art results on our dataset of textured meshes and on a dataset of distorted meshes with vertex colors. Finally, we present an application of our metric and dataset to explore the influence of distortion interactions and content characteristics on the perceived quality of compressed textured meshes. 

[*Full paper*](https://arxiv.org/abs/2202.02397)

## Variational Shape Reconstruction via Quadric Error Metrics
*Tong Zhao (Inria Sophia-Antipolis / Universite Cote d'Azur / LTCI, Telecom Paris), Laurent Buse, David Cohen-Steiner (Inria Sophia-Antipolis and Universite Cote d'Azur), Tamy Boubekeur, Jean-Marc Thiery (Adobe Research), Pierre Alliez (Inria Sophia-Antipolis and Universite Cote d'Azur)*

{{< figure src="Zhao2023.png" caption="Variational shape reconstruction. The clustering of the points is randomly initialized, then alternates partitioning and generator updating. Some generators relocate to sharp features after one iteration. New generators are then added. The clustering converges after five iterations. A set of candidate edges is derived from the adjacency between clusters, and candidate facets (red) are generated. The output mesh is reconstructed via a constrained binary solver that selects a subset of the red facets.">}}

Inspired by the strengths of quadric error metrics initially designed for mesh decimation, we propose a concise mesh reconstruction approach for 3D point clouds. Our approach proceeds by clustering the input points enriched with quadric error metrics, where the generator of each cluster is the optimal 3D point for the sum of its quadric error metrics. This approach favors the placement of generators on sharp features, and tends to equidistribute the error among clusters. We reconstruct the output surface mesh from the adjacency between clusters and a constrained binary solver. We combine our clustering process with an adaptive refinement driven by the error. Compared to prior art, our method avoids dense reconstruction prior to simplification and produces immediately an optimized mesh. 

[*Full paper*](https://hal.science/3IA-COTEDAZUR/hal-04131765v1)

## Somigliana Coordinates: An Elasticity-derived Approach for Cage Deformation
*Jiong Chen (Ecole Polytechnique), Fernando de Goes (Pixar Animation Studios), Mathieu Desbrun (Inria and Ecole Polytechnique)*

{{< figure src="Chen2023.png" caption="Somigliana coordinates. Given an initial cage (top inset) and its deformed pose, our novel cage deformer promotes a more elastic behavior of the cage deformation than previous works by leveraging an elasticity-derived matrix-weighted combination of both vertex positions and face normals of the cage. A Poisson ratio 𝜈 and bulging scale 𝛾 can be adjusted to offer control over local and global volume change.">}}

In this paper, we present a novel cage deformer based on elasticity-derived matrix-valued coordinates. In order to bypass the typical shearing artifacts and lack of volume control of existing cage deformers, we promote a more elastic behavior of the cage deformation by deriving our coordinates from the Somigliana identity, a boundary integral formulation based on the fundamental solution of linear elasticity. Given an initial cage and its deformed pose, the deformation of the cage interior is deduced from these Somigliana coordinates via a corotational scheme, resulting in a matrix-weighted combination of both vertex positions and face normals of the cage. Our deformer thus generalizes Green coordinates, while producing physically-plausible spatial deformations that are invariant under similarity transformations and with interactive bulging control. We demonstrate the efficiency and versatility of our method through a series of examples in 2D and 3D.

{{< video src="https://jiongchen.github.io/files/somi-video.mp4" controls="yes" >}}

[*Full paper*](https://jiongchen.github.io/files/somi-paper.pdf)

## Constraint-based Simulation of Passive Suction Cups
*Antonin Bernardin, Univ. Rennes / INSA / IRISA / Inria), Paul Kry (McGill University), Sheldon Andrews (Ecole de technologie superieure), Christian Duriez (Inria / Univ. Lille / CNRS), Maud Marchal (Univ. Rennes / INSA / IRISA / Inria)*

{{< figure src="Bernardin2023.png" caption="The Monster pop-up toy sticks to its base until the spring forces release it due to air leakage, making the whole structure to jump.">}}

In this paper, we propose a physics-based model of suction phenomenon to achieve simulation of deformable objects like suction cups. Our model uses a constraint-based formulation to simulate the variations of pressure inside suction cups. The respective internal pressures are represented as pressure constraints which are coupled with anti-interpenetration and friction constraints. Furthermore, our method is able to detect multiple air cavities using information from collision detection. We solve the pressure constraints based on the ideal gas law while considering several cavity states. We test our model with a number of scenarios reflecting a variety of uses, for instance, a spring loaded jumping toy, a manipulator performing a pick and place task, and an octopus tentacle grasping a soda can. We also evaluate the ability of our model to reproduce the physics of suction cups of varying shapes, lifting objects of different masses, and sliding on a slippery surface. The results show promise for various applications such as the simulation in soft robotics and computer animation.

{{< youtube id=PSKXglvD77I >}}

[*Full paper*](https://inria.hal.science/hal-03869711/)

## MesoGen: Designing Procedural On-surface Stranded Mesostructures
*Elie Michel, Tamy Boubekeur (Adobe Research)*

{{< figure src="Michel2023.jpg" caption="We propose a workflow for designing rich mesostructures, with self-similarity but no repetition artifacts. Our method is based on Wang tiling to enable fast authoring and efficient real-time rendering.">}}

Three-dimensional mesostructures enrich coarse macrosurfaces with complex features, which are 3D geometry with arbitrary topology in essence, but are expected to be self-similar with no tiling artifacts, just like texture-based material models. This is a challenging task, as no existing modeling tool provides the right constraints in the design phase to ensure such properties while maintaining real-time editing capabilities. In this paper, we propose MesoGen, a novel tile-centric authoring approach for the design of procedural mesostructures featuring non-periodic self-similarity while being represented as a compact and GPU-friendly model. We ensure by construction the continuity of the mesostructure: the user designs a set of atomic tiles by drawing 2D cross-sections on the interfaces between tiles, and selecting pairs of cross-sections to be connected as strands, i.e., 3D sweep surfaces. In parallel, a tiling engine continuously fills the shell space of the macrosurface with the so-defined tile set while ensuring that only matching interfaces are in contact. Moreover, the engine suggests to the user the addition of new tiles whenever the problem happens to be over-constrained. As a result, our method allows for the rapid creation of complex, seamless procedural mesostructure and is particularly adapted for wicker-like ones, often impossible to achieve with scattering-based mesostructure synthesis methods. 

{{< youtube id=AXDTo-JkECc >}}

[*Full paper*](https://eliemichel.github.io/MesoGen/documents/michel23mesogen.pdf)

## Fluid-solid Coupling in Kinetic Two-phase Flow Simulation
*Wei Li (Inria and Tencent Lightspeed Studios), Mathieu Desbrun (Inria and Ecole Polytechnique)*

{{< figure src="Li2023.png" caption="Key Drop. In this paper, we propose a stable and efficient kinetic two-phase flow simulator which can handle complex fluid-solid coupling, like a skeleton key being dropped in water. The dynamics of the bubbles entrapped by the fall is well captured as the insets of a real experiment demonstrate.">}}

Real-life flows exhibit complex and visually appealing behaviors such as bubbling, splashing, glugging and wetting that simulation techniques in graphics have attempted to capture for years. While early approaches were not capable of reproducing multiphase flow phenomena due to their excessive numerical viscosity and low accuracy, kinetic solvers based on the lattice Boltzmann method have recently demonstrated the ability to simulate water-air interaction at high Reynolds numbers in a massively-parallel fashion. However, robust and accurate handling of fluid-solid coupling has remained elusive: be it for CG or CFD solvers, as soon as the motion of immersed objects is too fast or too sudden, pressures near boundaries and interfacial forces exhibit spurious oscillations leading to blowups. Built upon a phase-field and velocity-distribution based lattice-Boltzmann solver for multiphase flows, this paper spells out a series of numerical improvements in momentum exchange, interfacial forces, and two-way coupling to drastically reduce these typical artifacts, thus significantly expanding the types of fluid-solid coupling that we can efficiently simulate. We highlight the numerical benefits of our solver through various challenging simulation results, including comparisons to previous work and real footage.

{{< video src="https://pages.saclay.inria.fr/mathieu.desbrun/Movies/LD23.mp4" controls="yes" >}}

[*Full paper*](https://pages.saclay.inria.fr/mathieu.desbrun/pubs/LD23.pdf)


## GREIL-Crowds: Crowd Simulation With Deep Reinforcement Learning and Examples
*Panayiotis Charalambous (CYENS - Centre of Excellence), Julien Pettre (Univ Rennes, Inria, CNRS, IRISA), Vassilis Vassiliades (University of Cyprus), Yiorgos Chrysanthou (CYENS - Centre of Excellence and University of Cyprus), Nuria Pelechano (Universitat Politecnica de Catalunya)*

{{< figure src="Charalambous2023.png" caption="Results from the same simulation - all agents use the pedestrian controller. The policy is able to capture and simulate simultaneously (a-d) social groups, flocks, individuals, mixed behaviours; (e-f) and various behaviors such as agents suddenly standing still, joining/leaving groups, etc. ">}}

Simulating crowds with realistic behaviors is a difficult but very important task for a variety of applications. Quantifying how a person balances between different conflicting criteria such as goal seeking,collision avoidance and moving within a group is not intuitive, especially if we consider that behaviors differ largely between people. Inspired by recent advances in Deep Reinforcement Learning, we propose Guided REinforcement Learning (GREIL) Crowds, a method that learns a model for pedestrian behaviors which is guided by reference crowd data. The model successfully captures behaviors such as goal seeking, being part of consistent groups without the need to define explicit relationships and wandering around seemingly without a specific purpose. Two fundamental concepts are important in achieving these results: (a) the per agent state representation and (b) the reward function. The agent state is a temporal representation of the situation around each agent. The reward function is based on the idea that people try to move in situations/states in which they feel comfortable in. Therefore, in order for agents to stay in a comfortable state space, we first obtain a distribution of states extracted from real crowd data; then we evaluate states based on how much of an outlier they are compared to such a distribution. We demonstrate that our system can capture and simulate many complex and subtle crowd interactions in varied scenarios. Additionally, the proposed method generalizes to unseen situations, generates consistent behaviors and does not suffer from the limitations of other data-driven and reinforcement learning approaches.

{{< youtube id=VNPUJJW4crM >}}

[*Full paper*](https://veupnea.github.io/publication_pages/siggraph23-greil.html)

## 3D Gaussian Splatting for Real-Time Radiance Field Rendering
*Bernhard Kerbl, Georgios Kopanas (Inria and Universite Cote d'Azur), Thomas Leimkuhler (MPI Informatik), George Drettakis (Inria and Universite Cote d'Azur)*

{{< figure src="Kerbl2023.png" caption="Our method achieves real-time rendering of radiance fields with quality that equals the previous method with the best quality [Barron et al . 2022], while only requiring optimization times competitive with the fastest previous methods [Fridovich-Keil and Yu et al . 2022; Müller et al. 2022]. Key to this performance is a novel 3D Gaussian scene representation coupled with a real-time differentiable renderer, which offers significant speedup to both scene optimization and novel view synthesis. Note that for comparable training times to InstantNGP [Müller et al. 2022], we achieve similar quality to theirs; while this is the maximum quality they reach, by training for 51min we achieve state-of-the-art quality, even slightly better than Mip-NeRF360 [Barron et al . 2022].">}}

Radiance Field methods have recently revolutionized novel-view synthesis of scenes captured with multiple photos or videos. However, achieving high visual quality still requires neural networks that are costly to train and render, while recent faster methods inevitably trade off speed for quality. For unbounded and complete scenes (rather than isolated objects) and 1080p resolution rendering, no current method can achieve real-time display rates.

We introduce three key elements that allow us to achieve state-of-the-art visual quality while maintaining competitive training times and importantly allow high-quality real-time (≥ 100 fps) novel-view synthesis at 1080p resolution.

First, starting from sparse points produced during camera calibration, we represent the scene with 3D Gaussians that preserve desirable properties of continuous volumetric radiance fields for scene optimization while avoiding unnecessary computation in empty space; Second, we perform interleaved optimization/density control of the 3D Gaussians, notably optimizing anisotropic covariance to achieve an accurate representation of the scene; Third, we develop a fast visibility-aware rendering algorithm that supports anisotropic splatting and both accelerates training and allows realtime rendering. We demonstrate state-of-the-art visual quality and real-time rendering on several established datasets. 

{{< youtube id=T_kXY43VZnk >}}

[*Full paper*](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/3d_gaussian_splatting_high.pdf)

[*Project page*](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/)

## PCBend: Light Up Your 3D Shapes With Foldable Circuit Boards
*Marco Freire\* (Universite de Lorraine / CNRS / Inria), Manas Bhargava\* (ISTA), Camille Schreck, Pierre-Alexandre Hugron (Universite de Lorraine / CNRS / Inria), Bernd Bickel (ISTA), Sylvain Lefebvre (Universite de Lorraine / CNRS / Inria) (\* Joint first authors)*

{{< figure src="Freire2023.png" caption="Starting from a 3D mesh our method automatically generates design files to produce an on-surface display composed of individually addressable RGB LEDs. The circuit board is manufactured through standard PCB production services, including component soldering. The user then folds the fabricated board back onto a 3D printed support. The final model becomes a curved display, onto which intricate light patterns can be programmed in a shader-like manner.">}}

We propose a computational design approach for covering a surface with individually addressable RGB LEDs, effectively forming a low-resolution surface screen. To achieve a low-cost and scalable approach, we propose creating designs from flat PCB panels bent in-place along the surface of a 3D printed core. Working with standard rigid PCBs enables the use of established PCB manufacturing services, allowing the fabrication of designs with several hundred LEDs. Our approach optimizes the PCB geometry for folding, and then jointly optimizes the LED packing, circuit and routing, solving a challenging layout problem under strict manufacturing requirements. Unlike paper, PCBs cannot bend beyond a certain point without breaking. Therefore, we introduce parametric cut patterns acting as hinges, designed to allow bending while remaining compact. To tackle the joint optimization of placement, circuit and routing, we propose a specialized algorithm that splits the global problem into one sub-problem per triangle, which is then individually solved. Our technique generates PCB blueprints in a completely automated way. After being fabricated by a PCB manufacturing service, the boards are bent and glued by the user onto the 3D printed support. We demonstrate our technique on a range of physical models and virtual examples, creating intricate surface light patterns from hundreds of LEDs.

{{< youtube id=nJspqdpyWq4 >}}

[*Full paper*](https://manas-avi.github.io/publications/2023/PCBend/FoldableElectronics-2023-camera-ready.pdf)

[*Project page*](https://visualcomputing.ist.ac.at/publications/2023/PLUY3SWFCB/)

## Fast GPU-based Two-way Continuous Collision Handling
*Tianyu Wang (FaceUnity), Jiong Chen (Ecole Polytechnique), Dongping Li, Xiaowei Liu (FaceUnity), Huamin Wang (Style3D), Kun Zhou (Zhejiang University)*

{{< figure src="Wang2023.png" caption="Knotting. The bow knot example (on the top, with 142K triangles) and the reef knot example (on the bottom, with 71K triangles) are presented. In this work, we develop a two-way method for safe and fast collision handling in deformable body simulation. Thanks to this method, our simulator can robustly handle complex collision contacts in these two examples at 4 to 17 FPS and 10 to 21 FPS respectively.">}}

Step-and-project is a popular method to simulate non-penetrating deformable bodies in physically-based animation. The strategy is to first integrate the system in time without considering contacts and then resolve potential intersections, striking a good balance between plausibility and efficiency. However, existing methods can be defective and unsafe when using large time steps, taking risks of failure or demanding repetitive collision testing and resolving that severely degrade performance. In this paper, we propose a novel two-way method for fast and reliable continuous collision handling. Our method launches an optimization from both ends of the intermediate time-integrated state and the previous intersection-free state. It progressively generates a piecewise linear path and eventually obtains a feasible solution for the next time step. The algorithm efficiently alternates between a forward step and a backward step until the result is conditionally converged. Thanks to a set of unified volume-based contact constraints, our method offers flexible and reliable handling of various codimensional deformable bodies, including volumetric bodies, cloth, hair and sand. Experimental results demonstrate the safety, robustness, physical fidelity and numerical efficiency of our method, making it particularly suitable for scenarios involving large deformations or large time steps.

{{< youtube id=6T52DU2iFu0 >}}

[*Full paper*](https://wanghmin.github.io/Wang-2023-FGB/Wang-2023-FGB.pdf)