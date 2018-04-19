# Install my R packages using drat

I am using this repository for users to be able to install my R package using the system drat http://eddelbuettel.github.io/drat/.

After installing the R package drat on their system, users can simply install one of my package by typing:

```{r}
drat::addRepo("courtiol")
install.packages("XXX") ## replace XXX by the name of the package!
```

This is work in progress but the packages will be added there progressively.
