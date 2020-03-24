# A template for external integration

NOTE: This is not a separate project. This is a derivative from
https://github.com/google/prog-edu-assistant.

This directory contains a skeleton setup for integration
of github.com/google/prog-edu-assistant to an external project.

How to use:

1. Copy the contents of this directory (`ext-notebook`) into
   an new empty project.

2. Run Bazel build to verify that the build setup works.

   ```shell
   bazel build ...
   # If setup works, the following file should be successfully generated.
   ls -l bazel-bin/helloworld-en-student.ipynb
   ```

3. Add your assignment notebooks (`.ipynb` files) and add build rules for
   them in `BUILD.bazel`, following the existing example.

4. Replace this `README.md` contents with the description of your project.

TODO(salikh): Implement generation of the autograding backend image.
TODO(salikh): Add local server and Cloud Run deployment instructions here.
