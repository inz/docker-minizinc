# Minimal MiniZinc Docker Images

_Find the images on Docker Hub at <https://hub.docker.com/r/inzinger/minizinc/>._

The [`update` script](./update) is run periodically and creates Docker images based on [Alpine 3.3](https://hub.docker.com/_/alpine/) for each MiniZinc release in the [MiniZinc releases feed](https://github.com/MiniZinc/libminizinc/releases).

## Using the Images

Run a MiniZinc model:

    docker run --rm -it -v $(pwd):/home -w /home inzinger/minizinc:2.0.13 minizinc path/to/model.mzn path/to/data.dzn

