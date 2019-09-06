# PyData NYC 2019 Tutorial on Neural Networks for Natural Language Processing

## Tutorial Overview
- Artificial Neural Networks, a recap of the past 50 years (10 minutes)
- The Building Blocks
  - Network Architecture
  - Scheduler
  - Optimizer
- Language and Recurrent Neural Networks
- Attention
- Memory Networks and Dynamic Memory Networks
- The Transformer Model


# Installation and Dependencies

You can use `docker` if you have it installed, if not you can also you `pipenv` to manage a local environment. For complete installation instructions for `pipenv` please refer to the `pipenv` documentation [here](https://docs.pipenv.org/en/latest/install/#installing-pipenv). Please make sure you are using Python 3.7.

### docker

Build the image, this will build the image (based on python 3.7) and install all required dependencies, including all the data required for the experiments.

```bash
chmod +x ./get_data.sh
./get_data.sh
docker build -t pydatanyc:latest ./
```

Start jupyterlab in a docker container

```bash
docker run -it -v $(pwd):/usr/src/app/ pydatanyc:latest jupyterlab
```


#### Errors

- [Errno 28] No space left on device
    - the docker deamon has run out of space, you need to clear old docker images / containers etc. from the system, a nuclear option for doing this is to run `docker system prune` but BE CAREFUL you will lose stopped containers.


### pipenv
```bash
git clone https://github.com/mattilyra/pydatanyc_2019
cd pydatanyc_2019
pipenv install
```

## Datasets


# Usage

If you're using `docker`, first start the container by

```
```
