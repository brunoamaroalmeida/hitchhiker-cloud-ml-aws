# The Hitchhiker's Guide to AI & ML in AWS workshop
### Getting started with AWS Sagemaker
> using the [AWS Labs MNIST K-Means example](https://github.com/awslabs/amazon-sagemaker-examples/tree/master/sagemaker-python-sdk/1P_kmeans_highlevel)

## STEPS
### 1. Create a Sagemaker Jupyter Notebook

Start by heading to the Sagemaker dashboard in AWS Console and create a Notebook instance.
![enter image description here](https://github.com/brunoamaroalmeida/hitchhiker-cloud-ml-aws/blob/master/sagemaker/images/1.%20CreateNB-1.png?raw=true)

Create a new IAM Role to use with that instance. Optionally you might want to give permissions to a specific bucket where your raw dataset is located.
![enter image description here](https://github.com/brunoamaroalmeida/hitchhiker-cloud-ml-aws/blob/master/sagemaker/images/1.%20CreateNB-2.png?raw=true)


Once your notebook is up and running, launch the Jupyer web interface.

![enter image description here](https://github.com/brunoamaroalmeida/hitchhiker-cloud-ml-aws/blob/master/sagemaker/images/1.%20CreateNB-3.png?raw=true)

### 2. Using AWS Labs MNIST K-Means notebook file

**2.1 Upload the example file to Jupyter**
Upload the ipython notebook to your Jypyter instance. You can find the file [here](https://github.com/awslabs/amazon-sagemaker-examples/blob/master/sagemaker-python-sdk/1P_kmeans_highlevel/kmeans_mnist.ipynb)


![enter image description here](https://github.com/brunoamaroalmeida/hitchhiker-cloud-ml-aws/blob/master/sagemaker/images/2.1%20Jupyter-1.png?raw=true)


**2.2 Following the steps in the notebook**

Select the cell and click Run to execute that python statement

![enter image description here](https://github.com/brunoamaroalmeida/hitchhiker-cloud-ml-aws/blob/master/sagemaker/images/2.2%20Jupyter-0.png?raw=true)

We start to inspect the data. Note that this is only one particular image and label from the entire dataset.
![enter image description here](https://github.com/brunoamaroalmeida/hitchhiker-cloud-ml-aws/blob/master/sagemaker/images/2.2%20Jupyter-1.png?raw=true)

You can tweak and show a different image & label
![enter image description here](https://github.com/brunoamaroalmeida/hitchhiker-cloud-ml-aws/blob/master/sagemaker/images/2.2%20Jupyter-2.png?raw=true)

In this section, you will start training the model...
![enter image description here](https://github.com/brunoamaroalmeida/hitchhiker-cloud-ml-aws/blob/master/sagemaker/images/2.2%20Jupyter-3.png?raw=true)

.... which triggers a training job in Sagemaker.
![enter image description here](https://github.com/brunoamaroalmeida/hitchhiker-cloud-ml-aws/blob/master/sagemaker/images/2.2%20Jupyter-3-1.png?raw=true)

After a few minutes the training is complete.
![enter image description here](https://github.com/brunoamaroalmeida/hitchhiker-cloud-ml-aws/blob/master/sagemaker/images/2.2%20Jupyter-4.png?raw=true)

Endpoint will be deployed and available to validate the model
![enter image description here](https://github.com/brunoamaroalmeida/hitchhiker-cloud-ml-aws/blob/master/sagemaker/images/2.2%20Jupyter-4-1.png?raw=true)

Validation for a single prediction
![enter image description here](https://github.com/brunoamaroalmeida/hitchhiker-cloud-ml-aws/blob/master/sagemaker/images/2.2%20Jupyter-5.png?raw=true)

Validation for a few clusters.
![enter image description here](https://github.com/brunoamaroalmeida/hitchhiker-cloud-ml-aws/blob/master/sagemaker/images/2.2%20Jupyter-6.png?raw=true)

### 3. Cleanup
There are a few resources that the AWS Labs example does not terminate. If might incur in unnecessary costs if you don't clean up the environment. Here is a step by step on how to do it.

Delete the S3 bucket
![enter image description here](https://github.com/brunoamaroalmeida/hitchhiker-cloud-ml-aws/blob/master/sagemaker/images/3.%20Cleanup-1.png?raw=true)

Delete the notebook instance
![enter image description here](https://github.com/brunoamaroalmeida/hitchhiker-cloud-ml-aws/blob/master/sagemaker/images/3.%20Cleanup-2.png?raw=true)

Delete the model
![enter image description here](https://github.com/brunoamaroalmeida/hitchhiker-cloud-ml-aws/blob/master/sagemaker/images/3.%20Cleanup-3.png?raw=true)


Delete the endpoint configuration
![enter image description here](https://github.com/brunoamaroalmeida/hitchhiker-cloud-ml-aws/blob/master/sagemaker/images/3.%20Cleanup-4.png?raw=true)
