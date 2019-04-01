# Example jobs and workflows
Each example can be run by typing:
```
prominence create <filename.json>
```

## job-raysect-lambert
Renders the image in the Raysect quick start guide, see: https://raysect.github.io/documentation/quickstart_guide.html. This examples uses a generic Raysect container with a user-provided input file containing the Python script to be executed. The output image is transferred to cloud storage.

## workflow-blender-demo
This is a 2 step workflow which renders frames from the Blender classroom demo (see https://www.blender.org/download/demo-files/) and creates a movie. B2DROP is used for storing the individual frames and final movie. This example also demonstrates multiple tasks in a single job (for deleting the individual frames after creating the movie).

Note that the B2DROP `app-username` and `app-password` need to be set in the JSON file. An application username and password can be generated on the B2DROP website.
