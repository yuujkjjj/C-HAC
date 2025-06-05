# :page_with_curl: Confidence-Guided Human-AI Collaboration: Reinforcement Learning with Distributional Proxy Value Propagation for Autonomous Driving

# :fire: Source Code Released! :fire:

## [[**arXiv**]](https://arxiv.org/abs/2506.03568)

1. This work introduces **Distributional Proxy Value Propagation (D-PVP)**, which integrates human intention into distributional reinforcement learning, enabling efficient policy learning with minimal human intervention.

2. A **shared control mechanism** and **policy confidence evaluation algorithm** dynamically balance human-guided and self-learning policies, ensuring both safety and performance in autonomous driving.

3. The proposed method is validated in both **MetaDrive** and **real-world urban driving** using a sensor-equipped UGV. Extensive experiments demonstrate superior performance in terms of sample efficiency, safety, and generalization across diverse traffic scenarios.

Email: lizeqiao@tju.edu.cn

# Framework

<p align="center">
<img src="https://github.com/lzqw/C-HAC/blob/main/pic/paper_framework_%E6%94%B9.jpg" height= "450" width="1000">
</p>


# Demonstration 

## Training example using C-HAC
[![Watch the vide](https://img.youtube.com/vi/_NIaXMbuRl8/0.jpg)](https://www.youtube.com/watch?v=uXmUke0Z1co)
## Testing example
[![Watch the vide](https://img.youtube.com/vi/_NIaXMbuRl8/0.jpg)](https://www.youtube.com/watch?v=_NIaXMbuRl8)
## C-HAC Real-World Driving Demonstration – Route 1
[![Watch the vide](https://img.youtube.com/vi/OwGJLFsqdjM/0.jpg)](https://www.youtube.com/watch?v=OwGJLFsqdjM)
## C-HAC Real-World Driving Demonstration – Route 2
[![Watch the vide](https://img.youtube.com/vi/CdV9UZtKCzM/0.jpg)](https://www.youtube.com/watch?v=CdV9UZtKCzM)

# User Guide

## Clone the repository.
cd to your workspace and clone the repo.
```
git clone https://github.com/lzqw/C-HAC.git
```

## Create a new Conda environment.
cd to your workspace:
```
conda create -n CHAC python=3.9
```

## Activate virtual environment.
```
conda activate CHAC
```

## Install Pytorch
Select the correct version based on your cuda version and device (cpu/gpu):
```
pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
```

## Install other requirements.
```
# Install the requirements.
pip install -r requirements.txt
```

## Training
Modify the sys path in **example_train** file, and run:
```
python train_dsact_pvp_rl.py
```




