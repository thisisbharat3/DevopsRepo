```
FROM: Specifies the base image.
COPY: Copies files from the host to the container.
ADD: Copies files from the host to the container (with additional features like URL support).
RUN: Executes commands to install dependencies or perform other setup tasks.
CMD: Specifies the default command to run when the container starts.
ENTRYPOINT: Sets the default executable for the container.
WORKDIR: Sets the working directory for subsequent instructions.
ENV: Sets environment variables.
ARG: Defines build-time variables.
EXPOSE: Exposes ports to the host machine.
LABEL: Adds metadata to the image.
MAINTAINER: Specifies the author or maintainer of the image (deprecated, replaced by LABEL).
USER: Sets the user or UID to use when running the container.
VOLUME: Creates a mount point and marks it as externally mounted.
HEALTHCHECK: Defines a command to check the container's health.
ONBUILD: Adds a trigger instruction to be executed when the image is used as the base for another build.
STOPSIGNAL: Sets the system call signal that will be sent to the container to exit
```
```
```
