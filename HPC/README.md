What is CUDA? 
CUDA is a model created by Nvidia for parallel computing platform and application programming interface. CUDA is the parallel computing architecture of NVIDIA which allows for dramatic increases in computing performance by harnessing the power of the GPU. 
What is Google Colab? 
Google Colab is a free cloud service and the most important feature able to distinguish Colab from other free cloud services is; Colab offers GPU and is completely free! With Colab you can work on the GPU with CUDA C/C++ for free!
CUDA code will not run on AMD CPU or Intel HD graphics unless you have NVIDIA hardware inside your machine.On Colab you can take advantage of Nvidia GPU as well as being a fully functional Jupyter Notebook with pre-installed Tensorflow and some other ML/DL tools.

To Run the CUDA program in COLAB:

Step 1: Go to https://colab.research.google.com in Browser and Click on New Notebook. 

Step 2: We need to switch our runtime from CPU to GPU. Click on Runtime > Change runtime type > Hardware Accelerator > GPU > Save.

Step 5: Now you can check your CUDA installation by running the command given below :
 

!nvcc --version

Step 6: Run the given command to install a small extension to run nvcc from the Notebook cells.

!pip install git+https://github.com/andreinechaev/nvcc4jupyter.git

Step 7: Load the extension using the code given below:

%load_ext nvcc_plugin

Step 8: Execute the code .


To Run the CUDA program in Ubantu (Terminal)

1. nvcc filename.cu 
2. ./a.out

To Run the CUDA program in CMD

1. g++ filename
2. ./a.out

