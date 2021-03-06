# XRAY-IMAGING
Analyzing X-Ray Imaging of potential covid-patient using deep learning

![XRAY](https://github.com/du00d/XRAY-IMAGING/blob/master/img/xray.png)

## Disclaimer
**The dataset was quite small (180 images each). I do not claim any diagonstic performance of the model this is simply an experiment inspired by this [paper](https://arxiv.org/abs/2004.05405)**

## Dependencies
* Tensorflow 2.0
* Keras
* Numpy 
* CV2

<code>pip install tensorflow</code> 
or <code>pip install tensorflow-gpu</code> (For the [GPU](https://www.tensorflow.org/install/gpu) accelerated version)

<code>pip install opencv-python</code>

## Datasets
XRAY Images of COVID Patients vs Normal (PA View)

The datasets are from [HERE](https://github.com/ieee8023/covid-chestxray-dataset) and [Kaggle](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia)

## Example

<code>python3 test.py sample.jpeg models/100accuracy</code>

The command above should print "Negative"

## Architecture
I was able to get a 100% accuracy on validation data, however it's likely due to a small dataset I did a 80/20 split for the dataset
![Architecture](https://github.com/du00d/XRAY-IMAGING/blob/master/img/architecture.png)
![alias](https://github.com/du00d/XRAY-IMAGING/blob/master/img/alias.png)

## Training
![Epoch accuracy](https://github.com/du00d/XRAY-IMAGING/blob/master/img/tensorboard.png)
![Epoch loss](https://github.com/du00d/XRAY-IMAGING/blob/master/img/tensorboard2.png)
