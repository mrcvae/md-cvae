# Mutually-Regularized Dual Collaborative Variational Auto-encoder for Recommendation Systems

 The codes are associated with the following paper:
 >**Mutually-Regularized Dual Collaborative Variational Auto-encoder for Recommendation Systems,**  
 >Anonymous Author(s),  
 >Submitted as a conference paper to IJCAI 2021.


## Environment

The codes are written in Python 3.6.5.  

- numpy == 1.16.3
- pandas == 0.21.0
- tensorflow-gpu == 1.15.0
- tensorflow-probability == 0.8.0

## Datasets

The processed datasets can be found [here](). 

For usage, copy the unzipped dataset folders into the data folder.

## Examples to run the codes
### 1. To reproduce the in-matrix prediction results:
- **Pretrain the dual item content embedding VAE**: 

    ```python pretrain_vae.py --dataset Name --split [0-9]```
- **Iteratively train the collarabotive and content VAEs**:

    ```python train_vae.py --dataset Name --split [0-9]```
- **Evaluate model and summarize the results into a pivot table**
    
    ```python predict.py --dataset Name --split [0-9]```
    
    ```python summarize.py```

### 2. To reproduce the out-of-matrix prediction results:
- Change to the cold_start folder.

- Download the processed data here [here]()**

- The way to run the codes and summarize the results is similar to the in-matrix case.

 **For advanced argument usage, run the code with --help argument.**