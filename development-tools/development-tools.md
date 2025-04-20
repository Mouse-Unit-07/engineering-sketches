# Development Tools
Below is a sketch of all tools used for development.

![Dev Tools](development-tools.drawio.png)

1. Fetch Docker image from JFrog Artifactory for development

2. Fetch source files from w/in Docker container to begin development

3. Fetch software packages from JFrog Artifactory if needed

4. Jenkins responds to pull requests on GitHub, and invokes Docker container to apply regression tests and build new binaries

5. Docker container fetches all packages currently on JFrog Artifactory to apply regression tests

6. Jenkins stores new binaries on JFrog Artifactory if source files are verified

7. Fetch micromouse testing software binary to run acceptance tests on micromouse hardware

8. Deploy firmware to micromouse over JTAG
