Graphics in Julia
========================================================
author: Andee Kaplan
date: 09-10-2014

Packages
========================================================

There are multiple packages written for Julia that facilitate graphics. The main difference between their use is the api syntax.

- [Winston](http://winston.readthedocs.org/en/latest/) (Matlab)
- [PyPlot](https://github.com/stevengj/PyPlot.jl) (Python matplotlib)
- [Gaston](https://github.com/mbaz/Gaston.jl) (gnuplot)
- [Gadfly](http://dcjones.github.io/Gadfly.jl/) (grammar of graphics)

Winston
========================================================
- ~~Static~~ 2D plotting library for Julia
- Syntax similar to Matlab


```r
using Winston

x = rand(10);
y = rand(10);
plot(x, y, "bo");

savefig("winston_plot.pdf");
```

Winston
========================================================
In order to print the plot, must save the plot, and insert into a `div` below.

<div align = "center">
  <object data="plots-julia/winston_plot.svg" type="image/svg+xml" width="600" height="400"></object>
</div>

Gaston
========================================================
- Wrapper for utilizing `gnuplot` from Julia


PyPlot
========================================================
- Wrapper for utilizing `matplotlib` (Python) from Julia




Gadfly
========================================================
- Implementation of the grammar of graphics in Julia
