# PyTorch & TensorFlow Local Setup for MPS on Apple Silicon Machines

This guide provides instructions to set up a local development environment for PyTorch and TensorFlow on Apple Silicon machines, specifically optimized for Metal Performance Shaders (MPS).

## Prerequisites

Make sure you have Conda installed on your system. If not, you can download and install it from [here](https://docs.conda.io/projects/conda/en/latest/user-guide/install/).

## Installation Steps

1. **Create a Conda Environment:**

   ```bash
   conda create --name env_pt_tf python=3.9 -y
   ```

2. **Activate Conda Environment:**

   ```bash
   conda activate env_pt_tf
   ```

3. **Install PyTorch:**

   Follow the official PyTorch installation guide [here](https://pytorch.org/get-started/locally/) to install PyTorch, torchvision, and torchaudio:

   ```bash
   conda install pytorch::pytorch torchvision torchaudio -c pytorch
   ```

4. **Install TensorFlow:**

   Install TensorFlow using the official Apple Metal plugin:

   ```bash
   python -m pip install tensorflow
   ```

5. **Install TensorFlow Metal Plugin:**

   ```bash
   python -m pip install tensorflow-metal
   ```

6. **Install Additional Packages:**

   ```bash
   conda install pandas jupyter jupyterlab scikit-learn matplotlib
   ```

7. **Launch Jupyter Lab:**

   ```bash
   jupyter lab
   ```

8. **Verify PyTorch Installation:**

   - Open and run [PyTorch_MPS_Checker.ipynb](PyTorch_MPS_Checker.ipynb) in Jupyter Lab.

9. **Verify TensorFlow Installation:**

   - Open and run [TensorFlow_MPS_Checker.ipynb](TensorFlow_MPS_Checker.ipynb) in Jupyter Lab.

10. **Verify Both Installations:**

   - Open and run [PyTorch_TensorFlow_Verification.ipynb](PyTorch_TensorFlow_Verification.ipynb) in Jupyter Lab.

## Resources

- [PyTorch Installation Guide](https://betterdatascience.com/pytorch-install/)
- [TensorFlow Metal Plugin](https://developer.apple.com/metal/tensorflow-plugin/)

Feel free to customize the setup according to your project requirements. Happy coding! 🚀
