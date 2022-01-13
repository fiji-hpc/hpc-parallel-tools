---
layout: default
---

# Welcome to the HPC-ParallelTools web portal!

![Animation Motivation](assets/images/motivationAnimation.gif)

## Motivation/Problem
Running image processing algorithms in parallel is desirable for image analysts and a major challenge for developers. As microscopy technology advances, users are facing larger and larger data volumes. One way to tackle the analysis of big image data is to split the image processing tasks into smaller sub-tasks and organize them for parallel execution in a High Performance Computing (HPC) facility.

While the cost of computational equipment decreases, making it possible to readily build or simply gain access to large HPC resources, the software able to exploit such hardware in a straightforward and user-friendly manner is lacking. 

## Solution
At IT4Innovations, we addressed this problem in Fiji by building a bridge to the prevalent HPC parallelization framework - the [Open MPI](https://www.open-mpi.org/).

In recognition of the diversity of ImageJ usage by the biology community, we enable Open MPI parallelization at two distinct levels within Fiji:

* Firstly, we enable parallelization of existing ImageJ macros through the Parallel Macro plugin. Parallel Macro can be used for progress reporting of tasks.
* Secondly, we implemented new Open MPI versions of some [ImageJ2 Ops](https://imagej.net/libs/imagej-ops/) -- atomic image processing commands that experienced developers can use to build complex image analysis solutions, called [OpenMPI Ops](https://imagej.net/plugins/openmpi-plugin-extensions) .

HPC-ParallelTools ease-of-use is achived by the [HPC Workflow Manager](https://imagej.net/plugins/hpc-workflow-manager) which provides a graphical user interface that automates the:
* creation of new jobs,
* uploading of data macros and scripts to the remote cluster, 
* submission of jobs, 
* downloading of results, 
* visual inspection of parallelized task progress, 
* live redirection of standard output and error output and editing of a job's macro or Jython script,
* use of the existing Fiji [Script Editor](https://imagej.net/scripting/script-editor) with added autocompletion support for the new parallelization and progress functions. 
* 
The HPC-ParallelTools framework delivers flexibility in parallelizing image processing tasks on large image sets or spatially large individual images without introducing additional complexity for casual users of ImageJ macro language or for experienced Java developers.

OpenMPI Ops can be combined with Parallel Macro to add another level of parallelization of Fiji Jython scripts. Parallel Macro and OpenMPI Ops are supported by HPC Workflow Manager.

## How to Start
If you have access to an HPC cluster and you are a new user, please read the [short guide](https://github.com/fiji-hpc/parallel-macro/wiki/Short-Guide). 

If you do not have access to an HPC cluster, you can try to [build and configure your own virtual cluster](https://github.com/fiji-hpc/parallel-macro/wiki/Building-Your-Own-Cluster-and-Configuring-It). You can download pre-made virtual hard drives for the [login node](https://helenos.fi.muni.cz/files/fiji-vm1.vdi), the [first compute node](https://helenos.fi.muni.cz/files/fiji-vm2.vdi) and [second compute node](https://helenos.fi.muni.cz/files/fiji-vm3.vdi), for all nodes the username is `fiji` and the password is `12345678`. Once you have set up a functional virtual cluster, you can go through the worksheets of the [short guide](https://github.com/fiji-hpc/parallel-macro/wiki/Short-Guide).
