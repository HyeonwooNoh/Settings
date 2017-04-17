# Setting AWS GPU Environment

#### Create EC2 Instance
I recommend to use 24GB SSD and to add [throughput optimized HDD](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EBSVolumeTypes.html?icmpid=docs_ec2_console).
Default setting (8GB SDD) is too small to install all of following dependencies.

For GPU environment, P2 instance is an appropriate choice [[reference](https://aws.amazon.com/ko/ec2/instance-types/)]

#### Install build essentials
```bash
sudo apt-get update && sudo apt-get upgrade
sudo apt-get install -y build-essential linux-image-extra-virtual
```

#### Setting & Mounting HDD
http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ebs-using-volumes.html

#### Setting NVIDIA CUDA Toolkit
http://docs.nvidia.com/cuda/cuda-installation-guide-linux/index.html#axzz4eUtSwdKs

#### Download CuDNN
https://developer.nvidia.com/rdp/cudnn-download

#### Install torch
http://torch.ch/docs/getting-started.html
