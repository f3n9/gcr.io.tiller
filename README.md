# gcr.io.tiller
## find out the latest version/tag of gcr.io image
- gcr.io/kubernetes-helm/tiller

## update Dockerfile with the new tag

## create a new release in github repo with name vX.YY.ZZ, e.g. v2.16.5

## goto https://cloud.docker.com/u/f3n9/repository/docker/f3n9/gcr.io.tiller and wait for the new image is built

## update version in CCS cluster.
helm init --upgrade -i f3n9/gcr.io.tiller:vX.YY.ZZ
