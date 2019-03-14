# Example jobs and workflows
The examples are run by typing:
```
prominence create <filename.json>
```

## workflow-blender-demo
This is a 2 step workflow which renders frames from the Blender classroom demo and creates a movie. B2DROP is used for storing the invididual frames and final movie. This example also demonstrates have multiple instances of the same job (in order to render the frames), and multiple tasks in a single job (for deleting the individual frames after creating the movie).
