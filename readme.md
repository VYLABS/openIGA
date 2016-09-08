openIGA code: openIGA provides NURBS wraped in Generic FEM commands

from the Computational Physics Group at the University of Michigan, adviser: Prof. Krishna Garikipati

current lead developer: Zhenlin Wang

List of contributors:

Zhenlin Wang

Shiva Rudraraju


Overview
=======================================================================
openIGA is a an isogeometric analysis based lib. It provides Nonuniform Rational B-Splines (NURBS) basis functions with generic finite element method commands for solving partial differential equations. Tt uses the automatic differentiation capabilities of the Sacado package from the Trilino library [https://trilinos.org/packages/sacado/], and it used deal.ii[www.dealii.org/download.html] for threads management. Currently the code is multi-threaded.


Version information
=======================================================================
This is version 0.1, the intial release of the code.


License
=======================================================================
GNU Lesser General Public License (LGPL). Please see the file LICENSE for details.



Acknowledgements
=======================================================================
This code has been developed under the support of the following:

1. NSF CDI Type I Grant: CHE1027729 “Meta-Codes for Computational Kinetics”

2. NSF DMREF grant: DMR1436154 “DMREF: Integrated Computational Framework for Designing Dynamically Controlled Alloy-Oxide Heterostructures”.



Installation with cmake:
=======================================================================
1. Install pre-required libs:

  1) Install CMake [http://www.cmake.org/download/]

  2) Install deal.II (version 8.4.1 recommended) with Trilinos [www.dealii.org/download.html]
     Deal.II OSX binaries include full packages of deal.ii with Trillions and other useful libs.


  3) Install Trillions [https://trilinos.org/] 
  

  4) Install hdf5 [https://www.hdfgroup.org/HDF5/]
  

  5) Install SuperLU [http://crd-legacy.lbl.gov/~xiaoye/SuperLU/]
  

2. Install openIGA lib
  1) Goes into “build” folder.
  2) Modify CMakeList.txt for path of pre-required libs: deal.ii (with Trilinos), hdf5, SuperLU,
  3) $ cmake CMakeLists
  4) $ make install
  5) $ make run
     - test(optional) of installation which will run “main” in build folder.
  6) “build” folder could be deleted after installation. 


Usage
=======================================================================
For usage of IGAlib, please see our specific applications:
defectsElastiticy:https://github.com/mechanoChem/defectsElasticity

data:08/22/2016
