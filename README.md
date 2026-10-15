# DeployWitness GitHub integration E2E

This public repository hosts disposable Docker Compose pull requests to verify the real reusable GitHub Actions workflow.

Both the reusable workflow and analyzer source are pinned to DeployWitness commit `e7d9cefe6982c596970dee4df6180343645c0a3f` (PR #15). The caller requests only `contents: read`; the workflow reads PR Git objects but never checks out or runs PR code. No secrets or production data are used.

Each scenario PR is tested against a fixed base and closed after recording its run. Standard `ubuntu-latest` public-repository runners are used.
