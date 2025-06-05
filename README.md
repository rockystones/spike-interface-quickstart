# spike-interface-quickstart
My quick start on using the spike interface project. 

It's an incredible project with tremendous group effort, the documentation is nice and detailed. But it is a little daunting for graduate students to start learning about it on their own without the help of experienced users, especially when we are not very coding savvy and familiar with using terminals/command lines. 

In addition, as the volume of document grow and the project evolving, some of it will inevitably become a little outdated and confusing. It will be even more frustrating for new users who are just starting.  

The hope of this quick start is the same as the "hello world!" when you are starting to learn coding.

Documenting my exploration with Version 0.102.3 project so others can learn from my experience. 

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

# Terminal for dummies
Getting familiar with using the terminal, especially the anaconda terminal/prompt/command line interface (or CLI)
https://www.lancaster.ac.uk/staff/drummonn/PHYS281/demo-terminal/
https://docs.conda.io/projects/conda/en/stable/user-guide/getting-started.html
https://docs.conda.io/projects/conda/en/stable/user-guide/cheatsheet.html

# IDE for dummies
You can't just keep typing code to the terminal all the time in real time. Hence the need for IDE/text editors, take your time with codings and then run everything all together.

Use Jupyternotebook: 
https://jupyter.org/install
https://docs.jupyter.org/en/latest/

# where do I start if I am using windows? 

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

### Quick tutorial

Start following the **Quickstart tutorial** to get the hello world running on demo data.

https://spikeinterface.readthedocs.io/en/stable/get_started/quickstart.html

Common issues, missing some package dependencies. 


### Get it working for my own data

### Install different sorters

Follow the recommendation using Docker because "Many of them come with several requirements that could cause conflicts in your Python environment."

https://spikeinterface.readthedocs.io/en/stable/get_started/install_sorters.html
https://spikeinterface.readthedocs.io/en/stable/modules/sorters.html#containerizedsorters
https://hub.docker.com/u/spikeinterface

Download and install Docker desktop for windows, register an account, login, update Docker if prompt. Then pull all the Docker images from spikeinterface Hub.

![image](https://github.com/user-attachments/assets/76bc2625-1605-41d3-80a9-c93b8272a762)
#### Docker for Dummies
https://www.docker.com/101-tutorial/
https://docker-curriculum.com/






# Does Linux work better?



