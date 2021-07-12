# ffpipeline
a Tekton pipeline that builds and outputs test results to a place

fork of https://github.com/bobcatfish/experimental/blob/pipeline-in-pod/pipeline-to-taskrun/examples/clone-test-upload.yaml Which tests for flakey tests by outputting to json and adding an additional task that evaluates json for signs of flakiness.

The jq for evaluation is currently somewhat contrived, it assumes that there are 2 tests in your test file.  But could easily be updated to be more robust.
