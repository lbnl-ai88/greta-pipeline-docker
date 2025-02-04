# greta-pipeline-docker

This repository provides a `compose.yaml` file for pulling down the `greta-pipeline` docker image, and running the basis generation code.

To run, clone the repository
```bash
git clone https://github.com/JessicaRehak/greta-pipeline-docker.git
```

Edit `config.yaml` to specify the steps you would like to run, edit any files in the `static_inputs/` directory, and then run

```bash
docker compose up
```

All the pipeline output files will be in `/output` by default. If you'd like to map a different location, edit the `source:` field under `volumes` in `compose.yaml`.