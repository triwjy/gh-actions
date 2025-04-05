Github Action

Building Blocks:
Workflow > Jobs > Steps

Required file structure to create a GH actions workflow:
  .github > workflows

Workflows: 
  - Are defined at the repository level
  - Define which triggers actually start the workflow
  - Are composed of one or more jobs

Jobs:
  - Are defined at the workflow level
  - Define in which execution environment they are run (linux, windows)
  - Will run in indenpendent VM (clean state) despite having the same environment
  - Are composed of one or more steps
  - Are run in parallel by default unless you specify the dependencies

Steps:
  - Are defined at the job level
  - Define the actual script or Github Action that will be executed
  - Run sequentially by default
