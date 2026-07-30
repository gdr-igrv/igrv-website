---
title: Des contributions françaises à SIGGRAPH 2026
date: 2026-07-30
draft: false
authors:
  - David Coeurjolly
  - Maud Marchal
---


La conférence [SIGGRAPH 2026](https://s2026.siggraph.org) a permis une mise en valeur de certaines contributions des laboratoires français. Sur la partie "Technical Papers" du programme, nous reprenons la liste des articles présentés à Los Angeles.

Notons également que deux articles : **Uncertainty-aware geometry processing on Gaussian Process Implicit Surfaces** (Baptiste Genest, David Coeurjolly) et **Implicit Minimal Surfaces for Bijective Correspondences** (Etienne Corman, Yousuf Soliman, Robin Magnet, Mark Gillespie) ont reçu un prix "Best Paper Award (Honorable Mention) lors de l'événement.

Enfin, l'article **Convolutional Wasserstein Distances: Efficient Optimal Transportation on Geometric Domains** SIGGRAPH 2015 (Justin Solomon, Fernando de Goes, Gabriel Peyré, Marco Cuturi, Adrian Butscher, Andy Nguyen, Tao Du, Leonidas Guibas) a quant à lui reçu un "Test-of-Time Award". 

N’hésitez pas à nous signaler tout oubli dans cette liste.


{{% toc %}}

## [Efficient Multiscale Lanczos Eigenpair Extraction](https://s2026.conference-schedule.org/?post_type=page&p=15&id=papers_1117&sess=sess127)

**Authors:**

- Theo Braune — Centre National de la Recherche Scientifique - Laboratoire d'informatique de l'École Polytechnique (LIX); Adobe Research
- Jérémie Dumas — Adobe
- Jean-Marc Thiery — Adobe

**Abstract:** We extend the implicitly restarted Lanczos method to a multiscale context using arbitrary multigrids (algebraic, geometric) and we demonstrate the gain in performance and robustness on a variety of application scenarios.

![Image teaser](https://s2026.conference-schedule.org/wp-content/linklings_snippets/representative_images/HqigTfKxdnzyUkPG.jpg)

## [Uncertainty-aware geometry processing on Gaussian Process Implicit Surfaces](https://s2026.conference-schedule.org/?post_type=page&p=15&id=papers_140&sess=sess149)

**Authors:**

- Baptiste Genest — CNRS; LIRIS
- David Coeurjolly — CNRS; LIRIS

**Abstract:** We present a geometry processing framework enabling computations directly on probabilistic representations of shapes. In contrast to classical geometry processing pipelines our approach considers uncertainty in the input data and account for the distribution of plausible geometries, enabling a principled handling of noise and ambiguity for downstream geometry processing tasks.

![Image teaser](https://s2026.conference-schedule.org/wp-content/linklings_snippets/representative_images/6R9MsJbeKDzuS8JA.jpg)

## [AtomSlicer: Constant-Thickness Field-Aligned Non-Planar Slicing and Continuous Toolpaths for FFF](https://s2026.conference-schedule.org/?post_type=page&p=15&id=papers_1058&sess=sess118)

**Authors:**

- Giovanni Cocco — Université de Lorraine, CNRS, Inria, LORIA
- Vincent Belle — Université de Lorraine, CNRS, Inria, LORIA
- Eric Garner — Université de Lorraine, CNRS, Inria, LORIA
- Sylvain Lefebvre — Université de Lorraine, CNRS, Inria, LORIA
- Xavier Chermain — Université de Lorraine, CNRS, Inria, LORIA

**Abstract:** AtomSlicer is a 3D printing method for fused filament fabrication that generates non-planar layers and continuous toolpaths aligned with user-defined fields. It enables better control of layer orientation, constant thickness, and near-continuous deposition, helping improve print quality, reduce interruptions, and support advanced multi-axis fabrication.

![Image teaser](https://s2026.conference-schedule.org/wp-content/linklings_snippets/representative_images/cU8Y4vKv6iVRmb5W.jpg)

## [SuperSDF:Sparse SDF Super-Resolution for Surface Extraction](https://s2026.conference-schedule.org/?post_type=page&p=15&id=papers_1060&sess=sess146)

**Authors:**

- Sagar Panwar — INRIA
- Nissim Maruani — INRIA
- Céline Loscos — L Research
- Mathieu Desbrun — INRIA
- Pierre Alliez — INRIA

**Abstract:** SuperSDF is a learning-based method for signed distance field super-resolution that reconstructs high-fidelity meshes from coarse inputs, without mesh supervision or auxiliary surface representations. Using a sparse voxel network near the surface, our approach learns how to directly refine the input SDF, outperforming prior methods in quality, efficiency, and scalability.

![Image teaser](https://s2026.conference-schedule.org/wp-content/linklings_snippets/representative_images/kxm1mQ96RgUmpGep.jpg)

## [Mechanical Cloaking of Halftoned Imagery](https://s2026.conference-schedule.org/?post_type=page&p=15&id=papers_1573&sess=sess118)

**Authors:**

- Jonàs Martínez — Inria
- Brisard Sébastien — Aix Marseille Université
- Kostas Danas — LMS, CNRS, Ecole Polytechnique
- Eric Garner — Inria
- Sid Kumar — TU Delft
- Sylvain Lefebvre — Inria

**Abstract:** We explore a new direction in mechanical cloaking: halftoning an image using a porous structure that behaves like a linear, isotropic material and visually matches an image. For an external observer, this creates the surprising effect where the object appears mechanically homogeneous while its porous structure resembles a target image.

![Image teaser](https://s2026.conference-schedule.org/wp-content/linklings_snippets/representative_images/e91Kw9HZQejBbFdT.jpg)

## [The PhaseTree: Multiphase Signed Distance Fields](https://s2026.conference-schedule.org/?post_type=page&p=15&id=papers_1372&sess=sess146)

**Authors:**

- Eric Galin — Université Claude Bernard Lyon 1; LIRIS
- Pierre Hubert-briere — Université Claude Bernard Lyon 1; LIRIS
- Marie-Paule Cani — Centre National de la Recherche Scientifique - Laboratoire d'informatique de l'École Polytechnique (LIX)
- Adrien Peytavie — Université Claude Bernard Lyon 1; LIRIS
- Eric Guérin — INSA, Lyon; LIRIS
- Hugo Schott — INSA, Lyon; LIRIS

**Abstract:** We introduce the PhaseTree, a novel hierarchical construction tree representation for compactly modeling objects composed of multiple phases or materials. An object is defined as a single tree that combines phase-aware primitives and operators, yielding a unified multiphase signed distance representation that naturally supports complex topologies and non-manifold interfaces.

![Image teaser](https://s2026.conference-schedule.org/wp-content/linklings_snippets/representative_images/65Fcp3ukLiwfMR7p.jpg)

## [Volume-Preserving LBM-MPM Coupling for Air-Water-Sand Mixtures](https://s2026.conference-schedule.org/?post_type=page&p=15&id=papers_297&sess=sess108)

**Authors:**

- Xiaoyu Xiao — Shanghai Jiao Tong University
- Haoxiang Wang — Department of Automation, Tsinghua University
- Xiaokang Yang — Shanghai Jiao Tong University
- Mathieu Desbrun — INRIA; Ecole Polytechnique
- Wei Li — Shanghai Jiao Tong University

**Abstract:** We present a physically-based framework for simulating sand–water–air mixtures by coupling LBM fluids with MPM granular sand under a unified formulation. A water retention model with built-in volume conservation enables stable, realistic simulation of mixtures across diverse, multiscale scenarios.

![Image teaser](https://s2026.conference-schedule.org/wp-content/linklings_snippets/representative_images/qmpJUVSehSsq1WHX.jpg)

## [Fast and Accurate Gaussian Process Modelling of Real-World Materials](https://s2026.conference-schedule.org/?post_type=page&p=15&id=paperstog_128&sess=sess130)

**Authors:**

- Arnau Colom — Pompeu Fabra University Interactive Technologies Group (GTI); Pompeu Fabra University, Interactive Technologies Group (GTI)
- Christian Bouville — Institut de Recherche en Informatique et Systèmes Aléatoires (IRISA)
- Julien Pettre — Institut National de Recherche en Informatique et en Automatique (INRIA) Rennes University, CNRS, IRISA
- Kadi Bouatouch — Institut de Recherche en Informatique et Systèmes Aléatoires (IRISA)
- Ricardo Marques — Pompeu Fabra University Interactive Technologies Group (GTI)

**Abstract:** We propose a BRDF modeling method that provides accurate and compact representations for isotropic and anisotropic BRDFs. We propose new theoretical developments enabling tractable Gaussian Process BRDF regression, leading to analytical BRDF representations. State-of-the-art methods can be outperformed in most BRDF cases by using a small training set of observations.

![Image teaser](https://s2026.conference-schedule.org/wp-content/linklings_snippets/representative_images/aodNT6g7pP8GoyXk.jpg)

## [Stochastic geomorphological transport for terrain erosion simulation](https://s2026.conference-schedule.org/?post_type=page&p=15&id=papers_735&sess=sess108)

**Authors:**

- Nicholas McDonald — erosiv Studio GmbH
- Guillaume Cordonnier — Inria, Université Côte d'Azur

**Abstract:** Geomorphological transport is the long-distance transport of quantities which are key elements of terrain erosion. We propose a new stochastic algorithm for the efficient simulation of geomorphological transport with momentum conservation, which enables us, for the first time, to model dynamic emergent deltas, meanders and debris fans in eroded terrains.

![Image teaser](https://s2026.conference-schedule.org/wp-content/linklings_snippets/representative_images/Qu3m7PqQNB7tikxh.jpg)

## [NILE: Nested Interleaving of Low-Dimensional Elements](https://s2026.conference-schedule.org/?post_type=page&p=15&id=papers_154&sess=sess124)

**Authors:**

- Abdalla Ahmed — Shenzhen University
- Matt Pharr — NVIDIA
- Victor Ostromoukhov — Université Claude Bernard Lyon 1; CNRS - LIRIS
- Hui Huang — Shenzhen University

**Abstract:** We introduce a novel modular modular meta-sampler architecture that bridges local subspace and global sampling, allowing integrator designers to employ specialized low-dimensional samplers while still achieving high-dimensional uniformity.

![Image teaser](https://s2026.conference-schedule.org/wp-content/linklings_snippets/representative_images/n2z4idWwG6w33tin.jpg)

## [NeuralSketch2Surf: Fast Neural Surfacing of Unoriented 3D Sketches](https://s2026.conference-schedule.org/?post_type=page&p=15&id=papers_1671&sess=sess116)

**Authors:**

- Hongsheng Ye — LTCI - Telecom Paris; Institut Polytechnique de Paris
- Anandhu Sureshkumar — LTCI - Telecom Paris; Institut Polytechnique de Paris
- Zhonghan Wang — LTCI - Telecom Paris; Institut Polytechnique de Paris
- Stefanie Hahmann — University Grenoble Alpes, CNRS, INRIA, Grenoble INP, LJK
- Marie-Paule Cani — LIX-Ecole Polytechnique/CNRS; Institut Polytechnique de Paris
- Georges-Pierre Bonneau — University Grenoble Alpes, CNRS, INRIA, Grenoble INP, LJK
- Amal Dev Parakkat — LTCI - Telecom Paris; Institut Polytechnique de Paris

**Abstract:** We introduce NeuralSketch2Surf, the first fast and robust neural surfacing solution, capable of processing arbitrary unoriented sketches at interactive rates.

![Image teaser](https://s2026.conference-schedule.org/wp-content/linklings_snippets/representative_images/j4s93GRoj4x5KPo8.jpg)

## [Explicit flows for implicit surfaces](https://s2026.conference-schedule.org/?post_type=page&p=15&id=papers_681&sess=sess184)

**Authors:**

- Camille Buonomo — CNRS - LIRIS
- Julie Digne — CNRS; LIRIS
- Raphaëlle Chaine — CNRS - LIRIS

**Abstract:** Our paper presents a method for shape-morphing and deformation using an exact mathematical flow. We introduce a neural architecture guaranteed to encode a flow, leveraging implicit supervision of explicit flows, ensuring topological consistency and efficient forward/inverse computation without ODE solvers. Applications include shape-morphing, editing, and transitions via a reference shape.

![Image teaser](https://s2026.conference-schedule.org/wp-content/linklings_snippets/representative_images/u19Rs7aNRjZByDuD.jpg)

## [Exact predicates, exact constructions and combinatorics for mesh CSG](https://s2026.conference-schedule.org/?post_type=page&p=15&id=paperstog_115&sess=sess122)

**Authors:**

- Bruno Levy — Inria Saclay and Laboratoire de Mathématiques d'Orsay Université Paris Saclay; INRIA, Saclay; Centre Inria de Saclay

**Abstract:** This article introduces an algorithm that exactly constructs the so-called Weiler model (also called a 3D mesh arrangement) and that uses it to implement CSG with arbitrary multi-operand expressions. The main contribution is a 2D Constrained Delaunay Triangulation with exact coordinates and symbolic perturbations to disambiguate configurations with co-cyclic points.

![Image teaser](https://s2026.conference-schedule.org/wp-content/linklings_snippets/representative_images/wJWN9sLcfDMWzTxA.jpg)

## [Implicit Minimal Surfaces for Bijective Correspondences](https://s2026.conference-schedule.org/?post_type=page&p=15&id=papers_1122&sess=sess129)

**Authors:**

- Etienne Corman — CNRS, Inria, LORIA
- Yousuf Soliman — Side Effects Software Inc
- Robin Magnet — INRIA; Université Paris Cité
- Mark Gillespie — INRIA; University of Utah

**Abstract:** We introduce an implicit representation of continuous, bijective, orientation-preserving maps between genus zero surfaces with or without boundary. The distortion of these maps can easily be minimized by optimizing the Ginzburg-Landau functional---a ubiquitous model in physics and differential geometry---leading to a simple algorithm for computing bijective correspondences using only standard tools of the tangent vector field toolbox. The method avoids combinatorial mesh modifications and does not require barrier functions to enforce bijectivity making it more robust to noise and simpler to implement.

![Image teaser](https://s2026.conference-schedule.org/wp-content/linklings_snippets/representative_images/hBAW1knFYUMyJWTn.jpg)
