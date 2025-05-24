# USLRA

This repo shows the source code of the paper: **Unified Semantic Space with Local Region Augmentation for Relation Triple Extraction**. To address these challenges, we propose a novel table filling RTE model based on **U**nified Semantic **S**pace and **L**ocal **R**egion **A**ugmentation (**USLRA**). 

## Running the Experiments

### Requirements

+ Python 3.8
+ PyTorch 1.7.1
+ transformers==4.5.1
+ pandas==2.0.3
+ numpy==1.24.4
+ GPU 3090



### Dataset
**NYT**. The NYT dataset is constructed using distant supervision for RTE tasks based on Freebase.

**NYT\***. The NYT* dataset is a partial annotation of the NYT dataset, where only the final token of an entity is labeled. 

**WebNLG**. The WebNLG dataset, originally introduced, was developed for natural language generation. It was later adaptedas a RTE benchmark. 

**WebNLG**. The WebNLG* dataset is a partial annotation of the WebNLG dataset, where only the final token of an entity is labeled. 

### How to run

#### Train

```bash
python main.py --dataset_name webnlg --lr 5e-5 --do_train ```
```

#### Test

```bash
python main.py --dataset_name webnlg --lr 5e-5 --do_eval ```
```





