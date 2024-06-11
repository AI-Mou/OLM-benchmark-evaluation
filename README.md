# OLM-benchmark-evaluation
This repo draws inspiration and references the ideas and code from https://github.com/huggingface/optimum-benchmark, with practical adjustments made for user convenience, allowing for direct and easy use within VS Code. Using microsoft/Phi-3-mini-4k-instruct as a case study, this repo independently verifies the performance of PyTorch inference and vLLM inference. 

For the tests, I used an Azure A100 VM as the experimental environment. The generated test reports are stored in the local file system of the Azure GPU VM.
```
Tue Jun 11 00:46:29 2024       
+---------------------------------------------------------------------------------------+
| NVIDIA-SMI 535.54.03              Driver Version: 535.54.03    CUDA Version: 12.2     |
|-----------------------------------------+----------------------+----------------------+
| GPU  Name                 Persistence-M | Bus-Id        Disp.A | Volatile Uncorr. ECC |
| Fan  Temp   Perf          Pwr:Usage/Cap |         Memory-Usage | GPU-Util  Compute M. |
|                                         |                      |               MIG M. |
|=========================================+======================+======================|
|   0  NVIDIA A100 80GB PCIe          On  | 00000001:00:00.0 Off |                    0 |
| N/A   34C    P0              43W / 300W |      9MiB / 81920MiB |      0%      Default |
|                                         |                      |             Disabled |
+-----------------------------------------+----------------------+----------------------+
                                                                                         
+---------------------------------------------------------------------------------------+
| Processes:                                                                            |
|  GPU   GI   CI        PID   Type   Process name                            GPU Memory |
|        ID   ID                                                             Usage      |
|=======================================================================================|
|  No running processes found                                                           |
+---------------------------------------------------------------------------------------+
```
You can run my code directly in VS Code, provided that you connect VS Code and the Azure GPU VM via a Jupyter server. Of course, you also have the option to run my code directly using Python.
I  compare the analysis results of PyTorch and vLLM inference for Phi-3-mini-4k-instruct on the A100 VM. 

