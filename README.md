# Devops-
Hadling Job Faiures:
Add a job using our favorite lightweight image, circleci/node:13.8.0.
Add a step that fails (on purpose). To do this, all you need is to exit with a non-zero code. That's easy with bash: return 1.
Define a second step that should only run if a previous step has failed. To do this, use the filter when: on_fail.
Define a workflow that uses the job.
Watch as your job fails, but runs your error handling step.
