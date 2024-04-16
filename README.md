# Exploration of a Reverse Turbo-Brayton Cryocooler for Carbon Neutral Aeronautical Applications

![python 3.2](https://img.shields.io/badge/version-latest-blue.svg) ![python 3.2](https://img.shields.io/badge/python-3.7-blue.svg) ![platform Linux,_MacOs,_Win64](https://img.shields.io/badge/platform-Linux,_macos,_win64-blue.svg)

The models and results from the MSc Thesis ["Exploration of a Reverse Turbo-Brayton Cryocooler for Carbon Neutral Aeronautical Applications"](https://repository.tudelft.nl/islandora/search/?collection=education) by Mik Swart. 

Performed at the Faculty of Aerospace Engineering of the Delft University of Technology, at the [Propulsion & Power research group](https://github.com/Propulsion-Power-TU-Delft).

---

## Repository Structure

The research, and therefore this repository, is structured as follows:

1. Liquid Hydrogen Fuel Tank
2. Reverse Turbo-Brayton Cryocooler System
3. Conceptual Compressor Design
4. Exploration Study

Each folder contains a readme file and two subfolders. These subfolders contain the code of the models, and the corresponding results.

## Author

__Mik Swart__, MSc Student, TU Delft

---

## Pre-requisites
##### [Modelica 4.0](https://www.modelica.org/)
##### [Dymola 2022](https://www.3ds.com/products-services/catia/products/dymola/) (not tested with OpenModelica)
##### [ExternalMedia](https://github.com/modelica-3rdparty/ExternalMedia)
##### [Python 3.9](https://python.org) (optional, only for Python - Dymola interface)
##### [NumPy](https://numpy.org) (optional, only for Python - Dymola interface)
##### [MatPlotLib](https://matplotlib.org) (optional, only for Python - Dymola interface)
##### [pandas](https://pandas.pydata.org/) (optional, only for Python - Dymola interface)
##### [tqdm](https://pypi.org/project/tqdm/) (optional, only for Python - Dymola interface)
##### [SMARTS 2.9.5](https://www.nrel.gov/grid/solar-resource/smarts.html) (optional, only for Python - Dymola interface)

---

## Setting Python - Dymola interface

The following instructions are tested for Python 3.7+ and Dymola 2022, assuming the Dymola installation folder to be the standard one.

1. Add to Path (environment variable): C:\\Program Files\\Dymola 2022\\bin64\\Dymola.exe

2. Create PYTHONPATH (environment variable), if not existing yet, and add: C:\Program Files\Dymola 2022\Modelica\Library\python_interface\dymola.egg

3. Set package_dir in main.py as "path-to-package.mo (inside DynTherM)" according to your system directory; set model_dir accordingly

4. Download SMARTS from NREL website and install it in the DynTherM root folder

    Upon completion of the previous steps, you should be able to run main.py from command line or python IDLE (remember to open the Dymola app before running main.py).
    The next step is only required to run main.py from PyCharm.

5. Open PyCharm and go to File/Settings/Project Interpreter. At the top right, select show all, show paths for the selected interpreter and add: C:\Program Files\Dymola 2022\Modelica\Library\python_interface/dymola.egg
