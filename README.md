# spike-interface-quickstart
My quick start on using the spike interface project. 

It's an incredible project with tremendous group effort, the documentation is nice and detailed. But it is a little daunting for graduate students to start learning about it on their own without the help of experienced users, especially when we are not very coding savvy and familiar with using terminals/command lines or GitHub. 

In addition, as the volume of document grow and the project evolving, some of it will inevitably become a little outdated and confusing. It will be even more frustrating for new users who are just starting.  

The hope of this quick start is the same as the "hello world!" when you are starting to learn coding.

Documenting my exploration with Version 0.102.3 project so others can learn from my experience. 

Two places I visited most often for answers: 
https://spikeinterface.readthedocs.io/
https://github.com/SpikeInterface

# A little note

### Motivation for trying this: 

I've got tons of ephys data to analyze. I don't want to do tons of manual curation. I am hoping the consensus of different sorters will help replace the manual sorting process. The time spend in learning about this project might end up being a lot less than myself manually curating hundreds of recording sessions. 

I am dealing with different file formats from different recording systems. Although many manufacture provide their data reading and exporting package, they are not easy to use. I am hoping at least the data interface module is useful in reading and exporting. Especially when we are required to publish the data in accessible format NWB.

I used the automated sorting from Plexon Offline SorterV3, and I am not very satisfied. I used early versions of Mountainsort, but it has to be running on Linux, not convenient for a lab that mostly use Windows desktops and workstations. 

### What beginners should expect: 

There is quite a learning curve. You should at least have some coding background, doesn't have to be Python, but enough to be comfortable reading the official doc and understand basic debugging process. Otherwise it will be too hard to learn it by yourself. It's better to find someone else who have use it before to collaborate on it. 

You will need a lot of time to troubleshoot. The docs were written by developers and experienced users, they might omit some details that seems too obvious to them but not to you. The demos are tested in running environment well tuned, but you will encounter errors/conflicts when setting up in your environment, or after you ran package updates. 

Focus on getting the basic demo running first, to help understand the structure and functions of the project. Then adapt to your own data, and later develop your own pipeline and workflow. 

Always refer to the official doc first for answers, then the GitHub issues, finally try to reach out to developers if you still cannot find anything. 

Developer community appreaciate many forms of contribution. https://spikeinterface.readthedocs.io/en/stable/development/development.html#how-to-contribute 

You will need to learn a bunch of new things but no need to be afraid. Bugs or error messages are not like running wet lab or animal experiments. Once you get comfortable using this open source tool, you will be more confident in trying out other open source tools and maybe one day release your own.

# Some background stuff to learn about in case you didn't already know

### Terminal for dummies
Getting familiar with using the terminal, especially the anaconda terminal/prompt/command line interface (or CLI)

https://www.lancaster.ac.uk/staff/drummonn/PHYS281/demo-terminal/

https://docs.conda.io/projects/conda/en/stable/user-guide/getting-started.html

https://docs.conda.io/projects/conda/en/stable/user-guide/cheatsheet.html

### IDE for dummies
You can't just keep typing code to the terminal all the time in real time. Hence the need for IDE/text editors, take your time with codings and then run everything all together.
https://wiki.python.org/moin/IntegratedDevelopmentEnvironments

### Use Jupyternotebook: 
Notebook vs IDE
https://afry.com/en/insight/data-science-in-notebooks-vs-ides
https://www.shiksha.com/online-courses/articles/jupyter-notebook-vs-python-idle/

https://jupyter.org/install

https://docs.jupyter.org/en/latest/

Jupyter note books are files using "ipynb" extension. 

Jupytext provides command line interface for converting notebooks between the different formats. https://jupytext.readthedocs.io/en/latest/using-cli.html
```
jupytext --to py notebook.ipynb                 # convert notebook.ipynb to a .py file
jupytext --to markdown notebook.ipynb           # convert notebook.ipynb to a .md file
jupytext --output script.py notebook.ipynb      # convert notebook.ipynb to a script.py file
jupytext --to notebook notebook.py              # convert notebook.py to an .ipynb file with no outputs
```

### GitHub for dummies

https://github.com/classroom-resources/github-starter-course

https://www.youtube.com/watch?v=8Dd7KRpKeaE

### Docker for Dummies
https://www.docker.com/101-tutorial/

https://docker-curriculum.com/

# Where do I start if I am using windows? 

Why I have to start from windows machine? Mac and Linux are great for coding and programming, but most equipment have better compatibility with windows. 

### Install the package
Start with installing anaconda and follow the beginner's instruction here.

https://spikeinterface.readthedocs.io/en/stable/get_started/installation.html#for-beginners

https://github.com/SpikeInterface/spikeinterface/tree/main/installation_tips

Download the **full_spikeinterface_environment_windows.yml**, and cd to where the yml is downloaded to run the installation within the conda virtual environment.
`conda env create --file full_spikeinterface_environment_windows.yml`

Activate the environment `conda activate si_env`
Download and run **check_your_install.py**
`python check_your_install.py`

![image](https://github.com/user-attachments/assets/de19980d-2546-4f8d-b32f-4068712d64f9)

![image](https://github.com/user-attachments/assets/8bab5106-1039-4a3d-bfbf-0bca7ce59878)

![image](https://github.com/user-attachments/assets/0ad80d19-995f-47e1-a577-1951556723b3)

### Install different sorters

Follow the recommendation using Docker because "Many of them come with several requirements that could cause conflicts in your Python environment."

https://spikeinterface.readthedocs.io/en/stable/get_started/install_sorters.html
https://spikeinterface.readthedocs.io/en/stable/modules/sorters.html#containerizedsorters
https://hub.docker.com/u/spikeinterface

Download and install Docker desktop for windows, register an account, login, update Docker if prompt. Then pull all the Docker images from spikeinterface Hub.

![image](https://github.com/user-attachments/assets/76bc2625-1605-41d3-80a9-c93b8272a762)

## Quick tutorial

Start following the **Quickstart tutorial** to get the hello world running on demo data.

https://spikeinterface.readthedocs.io/en/stable/get_started/quickstart.html

All the issues and error messages I came across are documented as issues in this GitHub repo. Most of them are easy to solve with solutions posted and then closed. When you ran into some issues, it is very likely they are already documented and solved, just search in the closed issues. 

![image](https://github.com/user-attachments/assets/0dfb5124-bcab-417c-be3b-988aa1bac87e)

Common issues, missing some package dependencies. 

Some errors are because the demo code was a little outdated. 

Some warnings and error messages are common and will likely happen very often in the future. Deprecation warnings, 

![image](https://github.com/user-attachments/assets/8c8d05a3-cb4a-4b93-b558-33ece96dac51)

### More demos to try 

Aside from this quickstart tutorial, there are quite a few Jupyter notebook demos you can try after you are done with the quickstart.  

Spikeinterface repo examples. https://github.com/SpikeInterface/spikeinterface/tree/main/examples
Many are what you see from the https://spikeinterface.readthedocs.io/
Many examples here are in the form of python script files with ".py" extension. Those "py" files you can directly run from the python kernel/terminal. 
You can use jupytext https://jupytext.readthedocs.io/ to convert from py script format to ipynb Jupyter notebook format.
`jupytext --to notebook <name_of_script_file>.py`

SpikeInterface Reports notebook collections
https://spikeinterface.github.io/ 

Spike tutorial repo https://github.com/SpikeInterface/spiketutorials/ 

This repo contains tutorials for using each package in spikeinterface. These tutorials range from basic to advanced and cover many powerful functionalities enabled by SpikeInterface.


### Get it working for my own data








# Does Linux work better?



