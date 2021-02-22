# The sequence in *Computational setup*

Generally speaking, we should write this part with a certain sequence. Since the readers might try to reproduce your results, or design their projects based on your paper, we'd better write this part in the sequence that we would follow in our projects.
For example, we should choose a **software package** for calcualtions, e.g. CP2K, VASP, etc.
Then, we should choose the **basis set** and the **pseudopotential** for the elements in our systems. 
...

Therefore, I write down the commonly used sequence here for convenience:

``` latex
% DFT setup
software package
basis set (polarization) and pseudopotential
energy cutoff
functional and dispersion correction
Gamma-point/k-point

% model build-up
slab size (test)
vacuum or water layer

% MD setup
MD method (e.g. BOMD, CPMD 2G-CPMD)
temperature and timestep
%% setup for 2G-CPMD
iteration number for OT
friction coefficient 
%% end setup for 2G-CPMD
time for equilibrium and production

% other setup ...

```
