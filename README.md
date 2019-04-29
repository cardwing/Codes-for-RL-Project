Codes for projects of IERG 6130 Reinforcement Learning

### Requirements

- Tensorflow 1.4.0
- MuJoCo 
- Gym 0.7.4

### Install necessary components
    conda create -n tensorflow_gpu pip python=2.7
    source activate tensorflow_gpu
    pip install --upgrade tensorflow-gpu==1.4
    pip install gym==0.7.4
    pip install mujoco-py==0.5.5
    
    
### Run the code
    source activate tensorflow_gpu
    cd PER-in-RL
    CUDA_VISIBLE_DEVICES=0 python run_ddpg_mujoco.py

### Notes
    export MUJOCO_PY_MJKEY_PATH=/path/to/mjpro131/bin/mjkey.txt
    export MUJOCO_PY_MJPRO_PATH=/path/to/mjpro131

You need to have the above mujoco key file in your path.

### Acknowledgement
This repo is built upon [Tensorflow-Reinforce](https://github.com/yukezhu/tensorflow-reinforce) and [prioritized-experience-replay](https://github.com/Damcy/prioritized-experience-replay)

