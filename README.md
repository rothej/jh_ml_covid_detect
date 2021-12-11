# jh_ml_covid_detect
ML project that detects COVID-19 infection from chest x-ray images.

Summary of Results:
The model was 99.9% accurate at detecting COVID infection when given a dataset of healthy and COVID-infected patient images.
The model performed poorly when Viral Pneumonia patient images were added, as the images were too similar for the model to classify accurately.
Switching from fitcecoc to a deeplearning CNN did not improve accuracy measurably. Either a more complex model, or more carefully processed input images, would likely be necessary (or both).

X-ray images obtained from: https://www.kaggle.com/preetviradiya/covid19-radiography-dataset

Main file list:
xray_cov_yn.mlx is the main MATLAB script used to train and test the COVID versus Healthy model.
xray_opt.mlx was ran to find optimal values (BoxConstraint and KernelValue).

Other files:
xray_cov_3class.mlx was the above MATLAB script with Viral Pneumonia images added (did not perform well).
xray_cov_3class_opt.mlx was ran to find optimal values (BoxConstraint and KernelValue).
xray_cov_deep.mlx was a script that used a basic deeplearning CNN to try to accomplish the 3-class task (also performed poorly).