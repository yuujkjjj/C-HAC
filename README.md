# :page_with_curl: Confidence-Guided Human-AI Collaboration: Reinforcement Learning with Distributional Proxy Value Propagation for Autonomous Driving

# :fire: Source Code Released! :fire:

## [[**arXiv**]]([https://www.researchgate.net/publication/382212078_Safety-Aware_Human-in-the-Loop_Reinforcement_Learning_With_Shared_Control_for_Autonomous_Driving](https://services.arxiv.org/html/submission/6510711/view))

1. This work introduces **Distributional Proxy Value Propagation (D-PVP)**, which integrates human intention into distributional reinforcement learning, enabling efficient policy learning with minimal human intervention.

2. A **shared control mechanism** and **policy confidence evaluation algorithm** dynamically balance human-guided and self-learning policies, ensuring both safety and performance in autonomous driving.

3. The proposed method is validated in both **MetaDrive** and **real-world urban driving** using a sensor-equipped UGV. Extensive experiments demonstrate superior performance in terms of sample efficiency, safety, and generalization across diverse traffic scenarios.

Email: lizeqiao@tju.edu.cn

# Framework

<p align="center">
<img src="https://github.com/lzqw/C-HAC/blob/main/pic/paper_framework_%E6%94%B9.jpg" height= "450" width="1000">
</p>


# Demonstration 

## Lane-change Performance
https://github.com/OscarHuangWind/Human-in-the-loop-RL/assets/41904672/690b4b44-ac57-4ce1-890b-57ac125cef63
## Uncooperative Road User
https://github.com/OscarHuangWind/Human-in-the-loop-RL/assets/41904672/52b2ec4b-8cd4-4b9d-a3a9-70bbd3b77157
## Cooperative Road User
https://github.com/OscarHuangWind/Human-in-the-loop-RL/assets/41904672/02f95274-80cc-4e6b-8a5b-edfcbbd4d0a6
## Unobserved Road Structure
https://github.com/OscarHuangWind/Human-in-the-loop-RL/assets/41904672/bb493f9c-d2c9-4db5-b034-ad456ef96c8a

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

## Install other rqquirements.
```
# Install the requirements.
pip install -r requirements.txt
```

## Training
Modify the sys path in **main.py** file, and run:
```
python example_train/train_dsact_pvp_rl.py
```




