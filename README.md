# ML-Quiz-XRay-ReportGeneration

Repository for ML-Quiz 

## Task 1
### Environments and Requirements
The full experiment id conducted in google colab. However, the experiment should be replicable in other common platform too.
- Python Version:  3.10.2

To install requirements:

```setup
pip install -r requirements.txt
```

### Dataset
Used the provided dataset.




### Run

To run the inference,

```python
jupyter nbconvert --to notebook --inplace --execute Task1.ipynb
```

The script will create a file named "Task1_Result.json" in the current directory. You can download the output file [here.](https://drive.google.com/file/d/19GW1Ih5PBacQNmf_my9SQ1NJLilklsx1/view?usp=sharing)

## Task 2
Task2 has three subparts,

- Part 1 : Fine tune
- Part 2 : Inference
- Part 3 : Evaluate

### Environments and Requirements
The full experiment id conducted in google colab. However, the experiment should be replicable in other common platform too.
- Python Version: 3.10.2

Each subpart has its own requiremnets. To install the requirements:

```setup
pip install -r requirements.txt
```
## Fine-tuning

Execute the fine-tuning script with:

```python
jupyter nbconvert --to notebook --inplace --execute Task2_Part1.ipynb
```
The model has been fine-tuned for 120 steps due to limited compute power. The fine-tuned model can be downloaded from [here.](https://drive.google.com/drive/folders/14NmCf0tt0gkL-aZSvMhPRNfXC9KJVuMZ?usp=sharing)

## Inference

To perform inference on the test and validation data splits, use:

```python
jupyter nbconvert --to notebook --inplace --execute Task2_Part2.ipynb
```
Due to limited compute resources, only 30% of the data is used for inference. The inference data is available [here](https://drive.google.com/file/d/1O-nDRfSCP9JN7DMpiN7arDVMbkLTicsP/view?usp=sharing) and [here.](https://drive.google.com/file/d/1-2xFqisCby0XSjWYylIURKsO1gyu7ZkY/view?usp=sharing)


## Evaluation

To evaluate the model on test and validation split, run this command:

```python
jupyter nbconvert --to notebook --inplace --execute Task2_Part3.ipynb
```
## Result
Here are the evaluation scores on different splits using [green score.](https://stanford-aimi.github.io/green.html) 
| **Data Split** | **Lung** | **Heart** | **Mediastinal** | **Bone** |
|:--------------:|:--------:|:----------:|:---------------:|:--------:|
|   Validation   |      0.3 |        0.4 |             0.4 |        0 |
|     Testing    |     0.45 |       0.44 |             0.6 |        0 |