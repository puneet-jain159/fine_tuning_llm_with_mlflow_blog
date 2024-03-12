# Fine Tuning LLMs with MLflow: Deep Learning with MLflow

This is a repo which contains the codes for  the blog ```Fine Tuning LLMs with MLflow: Deep Learning with MLflow (Part 2)``` These were on the Databricks Platform

## Runtime Tested
The following code is tested on ML DBR GPU 14.3 LTS Runtime

## Cluster Configurations
The Code to run open LLMS has been tested on the below single node cluster configurations:
- AWS : g5-24xlarge [4 A10's]
- Azure : NC24Ads_A100_v4 [1 A100]


## How to run the notebook:
1. Run the ```notebooks/data_prep.py``` to download the dataset from huggingface [here](https://huggingface.co/datasets/e2e_nlg) and store in dbfs.
2. Run the ```notebooks/run_deepspeed_fine_tuning.py``` to start the fine-tuning run and record the experiment.
3. Run the ```notebooks/run_inference.py``` to load any model checkpoint.