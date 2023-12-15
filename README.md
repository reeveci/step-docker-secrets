# Reeve CI / CD - Pipeline Step: Docker Secrets

This is a [Reeve](https://github.com/reeveci/reeve) step for setting up a docker volume with secret files.

This step creates a volume that contains secret files similar to how Docker swarm secrets work.
Howether, it uses generic docker volumes for this purpose, which allows changing their contents even while it is being used by running services.

The step set's a runtime variable that changes whenever the volume's contents are updated.
This can be used to automatically redeploy services when the secrets change.

## Configuration

See the environment variables mentioned in [Dockerfile](Dockerfile).
