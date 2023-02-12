# Particle_zoo_image_classification
The scope of this project is to build a CNN that can identify "particle zoo pins." Therefore, a robust dataset is in the works and a minimal and optimized neural network is under developement. This network is then going to be quantized using Qkeras. Then using the hls4ml workflow presented in the tutorial notebooks, ultimatley deploy the best algorithm on a Pynq-Z2 field programmable gate array(FPGA). Moreover, by using a generic webcam interfaced with the FPGA and the best trained model deployed on the board, we will perform "real-time" or "fastML" inference with minimal latency. 

The included notebooks are a general "sandbox" to begin loading the current data in the python notebook and storing it pythonically. The example.ipynb is the best place to start. The current CNN in this notebook is a great example of overfitting, and it is a good to get exeperience in resolving this common deep learning issue. A common solution to overfitting, is getting more data, openCV is a great resource in agmenting current image data and add it to the current data. 

I also have included a very messy image preprocessing notebook. I will be cleaing this up in the coming days and adding more on quantization in the example.ipynb. The goal for me in making this repository is to generate a common resource for future fastML demonstrations and orgranizing and integrating code that has been developed by my colleages at Fermilab and CERN. I hope that this repository can be used by future A3D3 postbacs, undergrads, and graduate researchers.  

# Starting up the notebook
command line on macOS or Linux: 
```
mkdir particle_zoo 
git clone https://github.com/A-Skiv/Particle_zoo_image_classification.git
conda env create -f particle_zoo_env.yaml
conda activate particle_zoo_env
jupyter notebook 
```
Have fun and enjoy the proccess! :)
