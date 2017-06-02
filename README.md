# OMPL (Open Motion Planning Library) plugin for V-REP

### Compiling

1. Install required python packages for [v_repStubsGen](https://github.com/fferri/v_repStubsGen): see v_repStubsGen's [README](https://github.com/fferri/v_repStubsGen/blob/master/README.md)
2. Install `xsltproc` (an XSLT processor)
3. Install `ompl`
4. Checkout and compile
```
$ git clone --recursive https://github.com/fferri/v_repExtOMPL.git
$ make
```

### Notes

#### Dubins state space

TurningRadius and symmetricity of Dubins Curve should be hardcoded due to the lack of parameter for `simExtOMPL_createStateSpace` (Line number 513: in `v_repExtOMPL.cpp`). (will be fixed in a future release)

