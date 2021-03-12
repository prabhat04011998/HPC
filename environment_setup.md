#Step-1

Login to Account
ssh -i <pem_file_name> <username>@10-10-119-10

#Load Modules in the Accound

module load compilers/anaconda/python3/2020.7
source /apps/compilers/anaconda3/etc/profile.d/conda.sh

#creating new environment for conda
conda create --name <nameOfEnv>

###after creating activate the environment
conda activate <name of env>

###command to remeber
conda deactivate
conda env list
conda list 

#Install the dependencies using the requirements.txt file.
conda install --yes --file requirements.txt
pip install -r requirements.txt


