
<a id='CHM.jl-1'></a>

# CHM.jl


A [Julia](http://julialang.org) package for extracting information from compiled help files (.chm).


<a id='Installation-1'></a>

## Installation


  * `Pkg.clone("https://github.com/PainterQubits/CHM.jl.git")`
  * This package requires a shared library. In the `deps` folder you can find a .dll file for Windows and a .dylib file for Mac OS X, either of which may or may not work for your computer. You will need to install the .dll file manually for now.


<a id='Quick-start-1'></a>

## Quick start


```
using CHM
f = CHM.open("/path/to/file.chm")
CHM.readdir(f, "/")
CHM.close(f)
```

