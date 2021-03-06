**Code and data for： <br />
Zhang^, Lengersdorff^, Mikus, Gläscher, & Lamm (2019, PsyArXiv). Frameworks, pitfalls, and suggestions of using reinforcement learning models in social neuroscience. (^Equal contributions)** <br />
[DOI: 10.31234/osf.io/uthw2](https://doi.org/10.31234/osf.io/uthw2).

___

This repository contains:
```
root
  ├─ code       # Matlab & R code to run the analyses and produce figures
  ├─ data       # behavioral & fMRI data
```

**Note 1**: to properly run all scripts, you may need to set the root of this repository as your work directory. <br />
**Note 2**: to reproduce the Matlab figures, you may need the [color brewer](https://www.mathworks.com/matlabcentral/fileexchange/34087-cbrewer-colorbrewer-schemes-for-matlab) toolbox and the [offsetAxes](https://github.com/anne-urai/Tools/blob/master/plotting/offsetAxes.m) function. 

## RL parameter simulations
* Figure 1A: [rl_learning_curve.m](code/rl_learning_curve.m) --> calls [simuRL_one_person.m](code/simuRL_one_person.m)
* Figure 1B: [rl_outcome_weight.m](code/rl_outcome_weight.m)
* Figure 1C: [plot_softmax.m](code/plot_softmax.m)
* Figure 1D: [rl_simulations.Rmd](code/rl_simulations.Rmd)

## fMRI time series of the prediction error
* Figure 2C: [pe_time_series_plot.m](code/pe_time_series_plot.m)
* core function: [ts_corr_basic.m](code/ts_corr_basic.m) --> relies on [normalise.m](code/normalise.m)
* permutation test: [ts_perm_test.m](code/ts_perm_test.m)

## posterior predictive check
* Figure 3A-C: [plot_ppc.m](code/plot_ppc.m)
* model fitting: [reinforcement_learning_HBA.R](code/reinforcement_learning_HBA.R) --> calls the stan model [rl_ppc.stan](code/rl_ppc.stan)


For bug reports, please contact Lei Zhang ([lei.zhang@univie.ac.at](mailto:lei.zhang@univie.ac.at)).

Thanks to this [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

___

### LICENSE

This license (CC BY-NC 4.0) gives you the right to re-use and adapt, as long as you note any changes you made, and provide a link to the original source. Read [here](https://creativecommons.org/licenses/by-nc/4.0/) for more details. 

![](https://upload.wikimedia.org/wikipedia/commons/9/99/Cc-by-nc_icon.svg)
