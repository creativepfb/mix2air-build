# mix2air-build

Public build recipe for the macOS version of a private project. It contains **only** the workflow file:
the private source code and the installers never live here.

How it works: a manual run clones the private repository using a secret token, builds on a GitHub macOS runner
(free for public repositories) and uploads the result to a private release repository.
Never upload build outputs as workflow artifacts here (artifacts of public repositories are public).
