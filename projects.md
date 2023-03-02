---
title: "Projects"
permalink: /projects/
---

## Projects

The projects I have been involved in regard various fields, topics and applications.
The problems I have dealt with are numerous and range from high-Mach compressible aeronautical flows, to highly turbulent low-Mach multiphase industrial flows and low-Reynolds incompressible pulsatile biological flows. Moreover, fluid-solid interaction and turbulence treatment, primarily through RANS computations and secondarily through DNS or LES, were also integral parts of my doctoral research at CITY, University of London.

#### Adaptive Mesh Refinement for Lattice Boltzmann Method
at _CEA_, 2021-2023

Apart from the "conventional" methods to resolve the systems of partial derivatives' equations that describe fluids' flows, namely finite volume, finite elements, finite differences, there exits the Lattice Boltzmann method.
According to this method, instead of solving the momentum and continuity equations (Navier-Stokes), the statistical Boltzmann equation for the out-of-equilibrium distribution system of fluid "particles" is solved.
Because the solution of this equation consists of two explicit steps (collision and relaxation), avoiding algebraic matrix operations and iterative algorithms, LBM is well suited for massive parallelism and HPC simulations.
The method is not mesh-free and is most commonly developed for Cartesian homogeneous regular grids.

This project focuses on developing a cross-platform LBM code with adaptive refinement capabilities, using [Kokkos](https://github.com/kokkos) library, for applications on porous media and multiphase flows.

#### Direct Forcing Immersed Boundary Method for OpenFOAM
at _CITY, University of London_, 2015-2020

An Immersed Boundary Method (IBM), a technique for modelling solid boundaries in the context of Computational Fluid Dynamics, was developed for cavitating and biological flows.
Modelling boundaries instead of meshing them, results in a far simpler computational domain and better quality computational grid. Problems with complex topologies or moving boundaries can be simulated in a simple Cartesian grid. Fluid-Structure Interaction problems with large deformations can especially benefit by IB techniques. The representation of the solid boundary take place with alternations in the numerical stencil of the discretised of the equations. Three approaches exist: direct forcing, ghost cell and cut cell; the _direct forcing_ method was followed, which essentially adds a volumetric source term in the momentum equation.

The aim was to create a tool suitable for a broad range of applications and flow regimes, from turbulent compressible cavitating industrial flows, to transitional incompressible biological flows. The method can be used for the simulation of needle movement in high pressure flows of Diesel injector nozzles, of rotating marine propellers, operating Mechanical Heart Valves in pulsatile blood flow or targeted drug delivery.

The method was developed within OpenFOAM, as a standalone dynamic library, achieving portability and extensibility. It can be integrated into different solution algorithms for different flow regimes, compiled as separate solvers within OpenFOAM. It has been validated for incompressible and cavitating solvers and tested for compressible and VOF solvers. It includes turbulence treatment through modified RANS models and accounts for flow induced motion.

<p align="center">
<img alt="free falling cylinder" src="https://mc08662.github.io/waterIcofallCyl05-w1ka1-mnml.gif" width="100%">
</p>

#### High speed solid-to-liquid impact
at _CITY, University of London_, 2019

A investigation of cavitation and shockwave dynamics upon the impact of a high speed projectile on a water jet was performed. This study tries to quantify the observations of a relevant experiment, and offer detailed information on vapour formation, pressure and velocity fields. Rich phenomena of schockwaves and liquid-gas interface interactions ware captured, including anomalous reflection of pressure waves, shock induced interfacial instabilities, as well as high speed jetting. The unveiled physics are in agreement with theoretical investigations and previous related research, however provide unique insight in the cavitation structures, both in 3D as well as 2D set-ups, and  valuable quantitative information about the impact and shockwave dynamics in a fast-slow configuration. The findings are related to bio-medical as well as industrial applications.
The experimental data were provided by collaborators in EPFL and the work resulted in publications in the [Int. Journal of Multiphase Flows](https://doi.org/10.1016/j.ijmultiphaseflow.2019.03.001) and at the 10<sup>th</sup> Int. Symposium on Cavitation [(CAV2018)](http://ebooks.asmedigitalcollection.asme.org/content.aspx?bookid=2565&sectionid=206551373) and a presentation during the 6<sup>th</sup> Cavitation Workshop [IICR 2019](http://iicr2019.net).

<p align="center">
<img alt="impact pressure waves" src="https://mc08662.github.io/logpGrad_blended-2.png" width="100%">
</p>

#### Wall shear stress on model aorta
at _CITY, University of London_, 2020

This project consists of numerical simulations of incompressible pulsatile flow through a model aorta to study vorticity structures and shear stress on the walls, to assist the calibration of a novel wall shear stress measurement technique, tailored for aortic flows. The flow as in transitional regime with the Reynolds number ranging from few hundreds to few thousands, and therefore the turbulence was not fully developed, prohibiting the use of RANS approach. This project was carried out in collaboration with an experimental team of CITY, who developed the measurement technique, and resulted in the composition of a scientific article, which is now in process of being submitted for publication.

#### Hybridization of experimental and computational flow data
at _ONERA, The French Aerospace Lab_, 2014

A method has been developed, which would merge numerical and experimental data. The aim was to benefit from the amount of information provided by numerical simulations on one hand, and from the accuracy of (limited) experimental measurements, on the other. Measurement campaigns on model aeroplanes in wind tunnels, are always considered more trustworthy than CFD. Therefore, the method ultimately tends to correct the computational data in order to provide a prediction of aeroplane's performance closer to "reality".

#### Supporting truss structure of WT blade
at _NTUA, National Technical University of Athens_, 2015

The project consists of an investigation of the possibility of replacing the default spar-beam support for the Wind Turbine blades, by a truss. The background idea was the potential use of such a truss structure in active control of the coupled fluid-structural system. The aim of the project was to define the procedure of determining the "equivalent beam" of the truss, used in aeroelastic simulations. The problem was approached by an inverse-design point of view and by well known means of optimization, in order to find the right material distribution along the equivalent beam and then define needed truss.

#### Non-engineering
##### Website development
at _CITY, University of London_, 2015-2018

Apart from the research works, as a member of _CaFE ITN_,  I had taken on the responsibility of set up and maintenance of the project's website _cafe-project.eu_ (the site now is inactive and archived). I used _Wordpress_ platform, as well as my elementary skills on `html` and `css`.
I also built the websites for two other similar ITN research projects coordinated by our laboratory, [HAOS ITN](http://haos-itn.eu/) and [IPPAD ITN](http://ippad-itn.eu/) (still active), and the websites of the annual international workshop on cavitation organised by our team in CITY, IICR2016 and [IICR2017](http://iicr2017.net/).
