
# RStudio + H2O

This Docker image meant to be a ready to use data science tools with h2o, rstudio and some additional useful packages.

The specific motivation is this docker should run examples in https://github.com/a-ghorbani/h2o_examples repository.
[This repo](https://github.com/a-ghorbani/h2o_examples) is cloned into guest user's home directory.

After running the docker you should be able to browse to http://localhost:8787, where you can get a web based r-studio. After login in using user `guest` and password `guest`, there should be a folder named h2o_examples-master. In this folder you can open R scripts and run it.

## Pull the image from Docker Repository

```
docker pull aghorbani/rstudio-h2o
```

## Running the image

```
docker run -it -p 8787:8787 -p 54321:54321 aghorbani/rstudio-h2o
```
