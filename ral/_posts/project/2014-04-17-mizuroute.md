---
layout: project
title:  "mizuRoute"
date:   2014-04-25 16:54:46
categories:
- project
- model
img: mizuRoute.png
img2: mizuRoute2.png
factsheet1: mizuRoute_1pg.pdf
factsheet2: mizuRoute_2pg.pdf
thumb: mizuRoute.png
client: USACE, USBR
website: http://blacktie.co
---

# A one-stop shop for routing streamflow

#### **The challenge:** 
 Hydrologic models generate runoff output that is spatially distributed, which then needs to be routed through the channel network to produce streamflow at a specific location. Existing continental domain portrayals of climate impacts commonly evaluate streamflow changes on a grid-based river network (left panel on figure) and typically use a single routing scheme and single parameter set to generate flow at limited gauge points. Additionally, different routing schemes work better in different locations (e.g., relatively flat locations benefit from more detailed dynamic simulations than places with a greater elevation gradient).

#### **Facing this challenge:**

Scientists and engineers at the Research Applications Laboratory (RAL) at the National Center for Atmospheric Research are collaborating with the US Army Corps of Engineers (USACE), Bureau of Reclamation, and University of Washington to build a multi-method, continental-domain routing model that efficiently routes streamflow from any distributed hydrologic model.  Called mizuRoute (in Japanese “mizu” means water), this software package is designed to quickly process large ensembles of future runoff at each time step to any location within the river network (illustrated below), facilitating spatial and temporal analysis that can be easily modified to address specific user needs.

#### **Scientific advances:**

mizuRoute provides a tool with a lot of flexibility and applications, including:
  * mizuRoute is a stand-alone software package that can be used with any spatially distributed hydrologic model output. It can be easily run in parallel and is well-suited for running large-ensembles.

  * mizuRoute can represent both a grid-type or vector-type river network (illustrated in the figure above).  One benefit of the vector river network is accurate representation of river length and contributing area, leading to more accurate streamflow.

  * mizuRoute can route streamflow for headwater basins, continental-wide river systems, and any desired location in the entire river network (not just pre-designated gauge points).   It currently produces values at 54,000 river segments across the contiguous United States based on the USGS Geospatial Fabric dataset, providing a more efficient and physically realistic alternative to gridded representations of the channel network. 

  * mizuRoute is developed in a modular framework. Therefore, multiple routing schemes can be implemented. mizuRoute currently has two routing schemes, one that includes more dynamics (kinematic wave tracking) and another that runs faster by using an impulse response function (unit hydrograph).

  * mizuRoute has a framework that allows for evaluation of routing scheme parameter sensitivity.  This is especially helpful for continental-domain applications, where continent-wide parameters do not exist. 

#### **Moving Forward:** 

These scientific advances provide opportunities to:

  * Simulate streamflow for hydrologic model evaluation, calibration, and future climate projections at locations most important to infrastructure design and operations.

  * Development is underway to add elements of water mass tracking, which would allow mizuRoute to be used in water quality evaluation (streamflow temperature, chemical constituents). 

  * Implementation of fuller dynamical routing, which would be more suitable for flat areas. To this end, a user could opt for whatever routing scheme is most appropriate, depending on the location (e.g., elevation gradients) and compute times, or multiple schemes to assess routing model uncertainty.
