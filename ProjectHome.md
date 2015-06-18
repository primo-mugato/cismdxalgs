A library of macros for the analysis software CISM-DX (a.k.a Open-DX). These tools were built primarily for studying the Lyon Fedder Mobarry global MHD code, although they also work for any global magnetosphere model that can be imported into DX. For details of the analysis techniques, see the draft of our paper on the Downloads page. Video tutorials for each of the example nets can also be found there.

The repository includes macros and tutorial nets for the following:

1) Obtaining cross sections of the LFM mesh, mesh joining and dipole mapping tools.

2) Construction of flux tube surfaces using connection elements of a curve and corresponding field line traces.

3) Construction of field line volumes, using connection elements of a surface and its corresponding field lines.

4) Using the above constructions, creating regions of interest parameterized by flux tube volume, potential, and normalized field line length.

5) A fast open/closed separatrix surface generator, which combines a 2D cell-splitting search with the 3D field-aligned volume construction. The tutorial also includes an open magnetic flux calculation.

Recent Updates (July 2010)

- Added tools for measuring vector and tensor flux through arbitrary surface meshes. The Flux macro now auto-detects whether the input is a vector field or tensor field and takes corresponding dot-products with each area element of the input surface. The user can specify whether the output fluxes should be cell-centered or vertex-centered. A metric input has also been added to help with unit conversions.

- Added LFMtensors macro, which converts any LFM 14-vector mhd field into components of the momentum equation, in mks or cgs units (user defined).

- Added tutorial that illustrates a few examples of tensor analysis in LFM, for a spherical region of interest.


TO DO:

- Implement line integrals for directed curves. Combine this with Flux analysis tools to enable easy path integration for the above surface constructions. Combine this with separatrix analysis.

- Implement volume integrals for regions of interest that are bounded by isosurfaces. Preferably, this should be done in a way that avoids stair casing artifacts near the boundary!