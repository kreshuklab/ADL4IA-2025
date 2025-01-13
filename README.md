# EMBL Advanced Deep Learning for Image Analysis 2025

## Schedule:

- Webinar 1: Monday 13th January  14:00 - 15:00 CET  
- Webinar 2: Monday 20th January  14:00 - 15:00 CET  
- Webinar 3: Monday 3rd February 14:00 - 15:00 CET  

## Set-up:

We will use on-premise EMBL resources (BARD) for the course. You can also use google colab to run the U-Net notebooks if you prefer. However, it might make sense to familiarise yourself with BARD as this is what you will be using during the course.

## BARD

You will all be given a login to a BARD account, working within this VM you can clone the git repo to your home folder and complete the exercises. More details will be given in precourse webinar 1 and can be found on the ecampus page or youcan always ask if you have other questions.

Running the exercises with BARD:
Login into your BARD account (The first login on a node may be slow)
Start VSCode by clicking its icon in the dock
Make sure vscode is in "Trust" mode, not "Restricted"
Install Python and Jupyter extensions
Go to Terminal-> new Terminal to start a terminal in vscode
IMPORTANT: It is best to only use the vscode terminal as it is inside a docker container that has access to git, conda and everything you need. Other terminals on BARD are in separate docker containers that don’t have access to everything. TLDR: just use the vscode terminal 🙂
In the terminal, 
git clone https://github.com/kreshuklab/ADL4IA-2025
cd into U-Net_exercise/pytorch
Open a .ipynb file in vscode
From the top right of vscode, ‘select kernel’ /opt/conda/envs/pytorch/bin/python

Note on wandb logging:
We are using wandb logging inside the notebooks as it is, in our opinion, nicer than tensorboard. Follow the instructions given by wandb when you run it to view your logs in a web browser.

You will need to login in wandb in order to start logging and will need to register if you don’t already have an account. The login is prompted in a cell at the beginning of every notebook although it will remember you after the first time. You can also login via the vscode terminal

 register with wandb and get a api key
in the terminal within vscode
source /opt/conda/etc/profile.d/conda.sh
conda activate pytorch
wandb login
 paste wandb api key and enter
 Run the notebook


Conda environments:
A few premade conda environments already exist within the docker container. These are read only. The pytorch environment will let you run all the pre-course exercises
The kernels/conda envs available are
/opt/conda/envs/pytorch/bin/python
/opt/conda/envs/keras/bin/python
/opt/conda/envs/sam/bin/python

These kernels/envs are read only. 

========
To create your own conda env
1. start a terminal in vscode
cd to your home directory
2. source /opt/conda/etc/profile.d/conda.sh
