# GitHub Actions Runner

[GitHub Actions Runner](https://github.com/actions/runner) runs GitHub Actions workflow jobs on your own hardware.
This app uses the [myoung34/github-runner](https://github.com/myoung34/docker-github-actions-runner) image,
which registers itself to a repository, organization or enterprise using a personal access token.

Target it from a workflow with **runs-on: [self-hosted, your-label]**.
Do not attach self-hosted runners to public repositories: a pull request from a fork could run arbitrary code on this system.

<!-- x-readme:warnings:start -->

⚠️ **WARNING:** This app has access to the Docker socket, which gives it full control over all containers and effectively root access to the system.

Misconfiguration or a malicious update can compromise data integrity, security, or system stability. Install at your own risk.

<!-- x-readme:warnings:end -->
