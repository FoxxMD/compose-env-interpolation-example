# ENVs and Variable Interpolation in Docker Compose

References:

* [Compose file interpolation](https://docs.docker.com/compose/how-tos/environment-variables/variable-interpolation/#env-file) and 
* [Environment variables precedence in Docker Compose](https://docs.docker.com/compose/how-tos/environment-variables/envvars-precedence/#how-the-table-works)
* [Set ENV variables within your container's environment](https://docs.docker.com/compose/how-tos/environment-variables/set-environment-variables/#use-the-env_file-attribute)

## Examples

### Default Compose File ENVs

```shell
docker compose up
```

* Uses `.env` since no other `--env-file` args
* Compose file does not define any env attributes for the service

Output is 

```
This is a variable:
```