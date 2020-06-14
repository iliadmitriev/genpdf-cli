# genpdf-cli

# build image

```
docker build -f Dockerfile -t genpdf-cli ./
```

# use

## Manual

```
docker run --rm --name genpdf-cli-run genpdf-cli -H
```

## Convert to pdf

```
docker run --rm --name genpdf-cli-run genpdf-cli -B 7 -T 7 -L 10 -R 10 -O Landscape \
       --zoom 0.95 --disable-smart-shrinking https://www.google.com/ - > google.pdf
```
