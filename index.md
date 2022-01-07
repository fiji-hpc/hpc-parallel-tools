# Welcome to the HPC-ParallelTools web portal!

Parallel Macro ([source code](https://github.com/fiji-hpc/parallel-macro)) is a plugin that enables the parallelization of existing ImageJ macro scripts, as well as progress reporting of tasks. 

Parallel Macro can be used in conjunction with [HPC Workflow Manager](https://imagej.net/plugins/hpc-workflow-manager) ([source code](https://github.com/fiji-hpc/hpc-workflow-manager-full)) which provides a graphical user interface that automates the creation of new jobs, uploading of data and scripts to the remote cluster, submission of jobs, downloading of results, visual inspection of parallelized task progress, live redirection of standard output and error output and editing of a job's macro or Jython script using the existing Fiji [Script Editor](https://imagej.net/scripting/script-editor) with added autocompletion support for the new parallel and progress functions. 

[OpenMPI Ops](https://imagej.net/plugins/openmpi-plugin-extensions) ([source code](https://github.com/fiji-hpc/scijava-parallel-mpi)) is a plugin which can be combined with Parallel Macro to add another level of parallelization of Fiji Jython scripts, OpenMPI Ops is also supported in HPC Workflow Manager.

If you have access to an HPC cluster and you are a new user, please read the [short guide](Short-Guide) first.

If you do not have access to an HPC cluster, you can try to set up and use a virtual cluster. The following page will guide you step by step in the task of [building your own cluster and configuring it](Building-Your-Own-Cluster-and-Configuring-It). Once you have set up a functional virtual cluster, you can go through the worksheets of the [short guide](Short-Guide).
