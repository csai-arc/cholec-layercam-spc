# Fused Multilayer Layer-CAM supervision for classification

This repository implements fused multilayer layer-cam supervision for classification.

### Train:

This package supports Imagefolder data format. To initiate the training, please use the below command.

 > python classification_training_layercam.py -a effnetv2_s --data <path to data> --epochs 5 --gpu-id 0 -c <path where checkpoints to be saved> --train-batch 10 --test-batch 1 --weights_load <path to pretrained weights> --optuna_study_db sqlite:///./<path where optuna db to be saved>
 
### Architecture Overview:

Utilized end to end encoder-decoder training architecture overview is given here.
<img src="/images/train_flow.PNG?" width="90%" >
  
Utilized inference architecture overview is given here.
<img src="/images/infer_flow.PNG?" width="90%" >

### Results:

Sample results on cholecystectomy is given below:
<img src="/images/surgery_analysis.png?" width="70%" >

Confusion matrix of surgical phase classification on cholec80 dataset is given below:
<img src="/images/confusion_matrix.png?" width="70%" >

Surgical Phase vs time plot is given below:
<img src="/evaluation_results/ribbon_plots.png?" width="70%" >






For trained network models please contact the author.
