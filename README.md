# Install my R packages using drat

I am using this repository for users to be able to install my R package using the system drat http://eddelbuettel.github.io/drat/.

This is work in progress but the packages will be added there progressively!


## For users:

Installing the R package {drat} on your system by running the following in your R console:
```{r}
install.packages("drat")
```

Then, simply install one of my package by running:

```{r}
drat::addRepo("courtiol")
install.packages("XXX") ## replace XXX by the name of the package!
```


## Tips for developers:

To include a package, do:

```{r}
drat::insertPackage(<path_tar_gz>, repodir = <path_drat_folder>)
```

To remove all packages from the drat folder, just do:

```{r}
drat::pruneRepo(repopath = ".", remove = TRUE)
```
