# Recommender Systems
Repo for my personal learning of Recommender Systems. Take anything in this repo with a grain of salt. :)

## Setup

1. `python3 -m venv .env`
1. `source .env/bin/activate`
1. `pip install -r requirements.txt`

## Running

1. source .env/bin/activate
1. jupyter lab

## Errors

If you get an error regarding Cuda not available this is due to suspend on Ubuntu 
with Nvidia. You need to run the following command:

```
sudo modprobe -r nvidia_uvm && sudo modprobe nvidia_uvm
```

If you get `FATAL: Module nvidia_uvm is in use` you need remove the usage:

```
sudo lsof /dev/nvidia*
```

I found that ollamma was calling all sorts of issues in my environment, I removed
this application.