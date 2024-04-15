# Robotic Fabrication in Architecture

## Welcome

Welcome to **Robotic Fabrication in Architecture**, a course dedicated to beginner-friendly creative coding sessions and exercises for building architecture with robots.

In these sessions, we will introduce computational methods for architecture, fabrication & construction, and incentivising computational literacy. Students will learn the theoretical background and basic implementation details of fundamental data structures and algorithms and plan and control robot tasks in CAD environments using the **[COMPAS](https://compas-dev.github.io/)** and **[COMPAS FAB](https://gramaziokohler.github.io/compas_fab/latest/)** framework, and other open-source libraries.


## Session Blocks

Title | Description | Slides  
----- | ----------- | ------
**Python Basics** | Quick start on Python | [Python Basics](https://docs.google.com/presentation/d/1fIpX7-DEaRLJhKe3QST4xTEx9U57yM9mbpVtvykUyD8/edit?usp=sharing)
**Geometry** | COMPAS geometry  | [Geometry](https://docs.google.com/presentation/d/16DmLj11qJGcRS9t2plSShqpEKF18fyEFxWbCWRyrwEE/edit?usp=sharing)
**Frames and Transformations** | Frames and transformations  | [Frames and Transformations](https://docs.google.com/presentation/d/1kMZ3cG7GBg3h3EDVvI_GPqTRwIeRn_IKUbUgkiBQ6sg/edit?usp=sharing)
**Data Structures** | COMPAS data structures  | [Data Structures](https://docs.google.com/presentation/d/1lRxruAAzjBgQr4ochBbuwnfC7lbJ6FwgH7dUbuNIuC0/edit?usp=sharing)
**Assembly** | Data structure for discrete assemblies  | [Assembly Information Model](https://docs.google.com/presentation/d/1EY5Ea9krgYT-yRucCcFmTMQWmW_tOlGJl_jmRUxw_n0/edit?usp=sharing)
**Robotic Assembly Planning** | Planning of a robotic assembly process | [Robotic Assembly Planning](https://docs.google.com/presentation/d/12F6xKzHDyGBA3t_Fu9rLMx7adLqFSEUbz4777dxN2UM/edit?usp=sharing)


## Requirements

* Windows 10 Professional
* Rhino 8 / Grasshopper
* [Anaconda Python](https://www.anaconda.com/download)
* [Visual Studio Code](https://code.visualstudio.com/)
* [Github Desktop](https://desktop.github.com/)
* [Docker Desktop](https://www.docker.com/products/docker-desktop)
* potentially: [Microsoft Visual C++](https://www.scivision.dev/python-windows-visual-c-14-required/)

After installing Rhino 8, open Rhino and run ScriptEditor on Rhino command line to initialize Python.

## Dependencies

* [COMPAS](https://compas-dev.github.io/)
* [COMPAS FAB](https://gramaziokohler.github.io/compas_fab/latest/)
* [Assembly Information Model](https://github.com/augmentedfabricationlab/assembly_information_model_2)
* [AM Information Model](https://github.com/augmentedfabricationlab/am_information_model_2)
* [UR Robot Simulation and Control](https://github.com/augmentedfabricationlab/ur_fabrication_control)

## Getting Started

Please set up your Python environment executing the commands below in Anaconda Prompt (Run as Administrator):

### 1. Setting up the Anaconda Environment with COMPAS FAB

#### Installation COMPAS FAB
    
    (base)  conda create -n rfab -c conda-forge compas_fab
    (base)  conda activate rfab

#### Verify Installation of COMPAS FAB

    (rfab) python -m compas_fab
    Yay! COMPAS FAB is installed correctly!   

#### Installation of COMPAS FAB on Rhino from PyPI

    (rfab) python -m compas_rhino.print_python_path
    (rfab) C:\Users\your_user_name\.rhinocode\py39-rh8\python.exe -m pip install compas_fab


### 2. Installation of Dependencies


#### Cloning the Course Repositories

Create a workspace directory:

C:\Users\YOUR_USERNAME\workspace

Then open Github Desktop and clone the following repositories into you workspace folder.

* [Robotic Fabrication in Architecture](https://github.com/le-ar-n/robotic_fabrication_in_architecture) 
* [Assembly Information Model](https://github.com/augmentedfabricationlab/assembly_information_model_2)
* [AM Information Model](https://github.com/augmentedfabricationlab/am_information_model_2)
* [UR Robot Simulation and Control](https://github.com/augmentedfabricationlab/ur_fabrication_control)


#### Making the Repositories Accessible in Rhino 8

Find the Rhino 8 Python executable by running the following in a terminal or command prompt:

    (rfab) python -m compas_rhino.print_python_path

Your Rhino 8 Python path should look something like this:

    C:\Users\your_user_name\.rhinocode\py39-rh8\python.exe
    

Then you can pip install all dependencies using the file path of the Rhino 8 Python executable:

    (rfab) your_py39-rh8_path -m pip install your_filepath_to_assembly_information_model

    (rfab) your_py39-rh8_path -m pip install your_filepath_to_am_information_model

    (rfab) your_py39-rh8_path -m pip install your_filepath_to_ur_fabrication_control

**Voilà!**
**You can now go to VS Code, Rhino or Grasshopper and run the example files!**
