# spike-interface-quickstart
My quick start on using the spike interface project 

It's an incredible project with tremendous effort, the documentation is nice and detailed, but still, it is a group effort, as the volume of document grow, some of it will be confusing, and it is a little daunting for graduate students to start learning about it on their own without the help of experienced users, especially when we are not very coding savvy and familiar with using terminals/command lines. 

The hope of this quick start is the same as the "hello world!" when you are starting to learn coding. 

Documenting my exploration with the project so others can learn from my experience. 

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



