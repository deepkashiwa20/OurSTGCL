# OurSTGCL

### Requirements
My settings are python=3.9.17, torch=1.10.0+cu111, **scipy=1.11.1**

```
python3 -m pip install -U scipy
```

## Dataset
Generate the training, validation and test sets by using:
##### METRLA
```
python generate_training_data.py 
```
##### PEMSBAY
```
cd PEMSBAY
unzip *.zip
cd ..
python generate_training_data.py --dataset PEMSBAY --output_dir PEMSBAY/ --traffic_df_filename PEMSBAY/pems-bay.h5
```


## Run

#### joint-graph

```
cd joint-graph
python train.py --dataset METRLA
```
#### joint-node
```
cd joint-node
python train.py --dataset METRLA
```
