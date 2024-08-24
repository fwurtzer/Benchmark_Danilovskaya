# Benchmark 2nd problem Danilovskaya

[![GitHub license](https://img.shields.io/github/license/fwurtzer/Benchmark_Danilovskaya2)](https://github.com/fwurtzer/Benchmark_Danilovskaya2) [![GitHub release](https://img.shields.io/github/release/fwurtzer/Benchmark_Danilovskaya2.svg)](https://github.com/fwurtzer/Benchmark_Danilovskaya2/releases/) 

## 1) Description

This repository contains an [NGSolve](https://ngsolve.org/) implementation of the second Danilovskaya problem [^1], which is a classical strongly coupled thermo-elasticity benchmark detailed by [Shu & Stanciulescu](https://www.doi.org/10.1061/(ASCE)EM.1943-7889.0001669) [^2].


## 2) Quickstart

- To run **online** with [Binder](https://jupyter.org/binder) (no installation required):
  - click on the following Binder link [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/fwurtzer/Benchmark_Danilovskaya2/main?urlpath=/tree/)
  - wait for the launch of the virtual machine
  - click on `ThermoElasticity.ipynb`

- To run **locally** (installation required):
  - clone the repository or download its content (click on `Code <>`, then `Download ZIP`)
  - follow the installation instruction given hereafter
  - run `ThermoElasticity.ipynb`

## 3) Local installation (tested on Windows 10 and 11)

1. Download and unzip the contents of the current [github directory](https://github.com/fwurtzer/Benchmark_Danilovskaya2) in any folder. Click on `Code <>`, then `Download ZIP`.
2. Download and install [Miniconda](https://docs.conda.io/en/latest/miniconda.html) with the default options for your system.
3. Open an Anaconda Prompt console (on Windows, type `Anaconda prompt` in the bottom-left search bar; on Linux and Mac, use the terminal directly).

From now on, write the following sequence of instructions on the console (you can copy the instructions and paste them into the console by right-clicking; press Enter after writing the instruction to execute it; press “y” to confirm when prompted) : 

4. Create a new environment called “benchmark_Danilovskaia” : `conda create -n benchmark_Danilovskaia python=3`.
5. Activate the environment: `conda activate benchmark_Danilovskaia`.
6. Install the necessary packages (500Mb): `conda install jupyter numpy matplotlib` (press `y` + `Enter` to confirm installation). If a freeze occurs, close the console and repeat steps 3, 5 and 6. Packages already downloaded will not be re-downloaded, which will make the process smoother.
7. Install NGSolve (300Mb): `pip install ngsolve`.
8. Install viewing extensions on notebooks:
 - `pip install --upgrade webgui_jupyter_widgets`
 - `jupyter nbextension install --user --py webgui_jupyter_widgets`
 - `jupyter nbextension enable --user --py webgui_jupyter_widgets`

9. Launch Jupyter: `jupyter notebook`.
10. In the file explorer that opens, select the folder where the code was download, and run `ThermoElasticity.ipynb`. 

## 4) Citation

Please use the following citation reference if you use the code:

    F. Wurtzer, T. Cherrière. Github repository: fwurtzer/Benchmark_Danilovskaya2 (v1.0), August 2024. Zenodo. URL ZenodoXXX

## 5) License

Copyright (C) 2024 Floriane WURTZER (floriane.wurtzer@ens-paris-saclay.fr), Théodore CHERRIÈRE (theodore.cherriere@ricam.oeaw.ac.at)

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this program.  If not, see <https://www.gnu.org/licenses/>.

[^1]: Danilovskaya, V. (1952). *On a dynamic problem of thermoelasticity*. In Prikladnaya Matematicka i Mekhanika (Vol. 16, Issue 4, pp 341-344).
[^2]: Shu, W., & Stanciulescu, I. (2019). *Monolithic and Staggered Strategies Using Solid-Shell Formulations for Nonlinear Coupled Thermoelasticity*. In Journal of Engineering Mechanics (Vol. 145, Issue 12). American Society of Civil Engineers (ASCE). DOI : [10.1061/(asce)em.1943-7889.0001669](https://doi.org/10.1061/(asce)em.1943-7889.0001669)
