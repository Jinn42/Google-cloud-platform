# Google-cloud-platform

# Jupyter notebook
## Objective: To run youy own Jupyter Notebook on Google Cloud Platform (GCP)
1. To generate an SSH keypair(if you don't have yet )
To create a SSH keypair named jupyter

```
ssh-keygen -t rsa -b 4096 -C jupyter -f jupyter
```
![](https://github.com/Jinn42/Google-cloud-platform/blob/main/ssh_key.png)

2. Create VM instance
![](https://github.com/Jinn42/Google-cloud-platform/blob/main/conf1.png)
![](https://github.com/Jinn42/Google-cloud-platform/blob/main/spasted-image-2.png)
![](https://github.com/Jinn42/Google-cloud-platform/blob/main/conf3.png)

3. Install notebook package
connect by SSH:
![](https://github.com/Jinn42/Google-cloud-platform/blob/main/connect_ssh.png)
```
sudo apt-get update
sudo apt install python3-pip
pip3 install Jupyter
export PATH=$PATH:~/.local/bin
source ~/.bashrc
jupyter notebook --no-browser
```
4. Access jupyter notebook
![](https://github.com/Jinn42/Google-cloud-platform/blob/main/jupyter_browse.png)
access by the url given on the last image:
http://localhost:8888/?token=058cc4458cf60ad2b3efa9c07343449715a29300f9763d3a

