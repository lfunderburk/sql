## Set up - with Docker

```
docker build -t movierec:latest -f Dockerfile .
docker run -it movierec:latest
```

## Set up - one step at a time

1. Create new environment

```
conda create --name poetry-env python=3.10
```

2. Activate environment

``` 
conda activate poetry-env
```

3. Install poetry

```
pip install poetry
```

4. Install dependencies

```
poetry lock
poetry install
```

5. Run the as a Ploomber pipeline

```
cd mini-projects/
poetry run ploomber build
```

