# Example jobs and workflows

## Raysect
### job-raysect-lambert
Renders the image in the Raysect quick start guide, see: https://raysect.github.io/documentation/quickstart_guide.html. This examples uses a generic Raysect container with a user-provided input file containing the Python script to be executed. The output image is transferred to cloud storage.

## Blender
### workflow-blender-demo
This is a 2 step workflow which renders frames from the Blender classroom demo (see https://www.blender.org/download/demo-files/) and creates a movie. B2DROP is used for storing the individual frames and final movie. This example also demonstrates multiple tasks in a single job (for deleting the individual frames after creating the movie).

Note that the B2DROP `app-username` and `app-password` need to be set in the JSON file. An application username and password can be generated on the B2DROP website.

## OSPRay
### ospray-streamlines-demo.ipynb
This is the NASA Streamlines demo from http://www.ospray.org/demos.html. PROMINENCE is used to do an offline render.

Here we access PROMINENCE entirely from a Juypter notebook. The example notebook was created on Google Colab but any other Jupyter platform can be used.

## LAMMPS
### lammps-bench-single
This runs sequentially the 5 benchmark problems described here: https://github.com/lammps/lammps/tree/master/bench. These are the serial one processor runs.

To run this example, type:
```
prominence run https://raw.githubusercontent.com/prominence-eosc/examples/master/lammps-bench-single.json
```

### lammps-bench-fixed-size-single-node
This runs sequentially the 5 benchmark problems described here: https://github.com/lammps/lammps/tree/master/bench. These are the parallel fixed-size runs using 8 cores on a single node using Open MPI.

To run this example, type:
```
prominence run https://raw.githubusercontent.com/prominence-eosc/examples/master/lammps-bench-fixed-size-single-node.json
```

### lammps-bench-fixed-size-single-node-openmp
This runs sequentially the 5 benchmark problems described here: https://github.com/lammps/lammps/tree/master/bench. These are the parallel fixed-size runs using 8 cores on a single node using OpenMP.

To run this example, type:
```
prominence run https://raw.githubusercontent.com/prominence-eosc/examples/master/lammps-bench-fixed-size-single-node-openmp.json
```
### lammps-bench-hybrid
This runs sequentially the 5 benchmark problems described here: https://github.com/lammps/lammps/tree/master/bench. These are the parallel fixed-size runs using two 4-core nodes using both Open MPI and OpenMP, i.e. OpenMP is used to run multiple threads per MPI task.

To run this example, type:
```
prominence run https://raw.githubusercontent.com/prominence-eosc/examples/master/lammps-bench-hybrid.json
```
