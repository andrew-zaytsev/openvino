# Model Optimizer Developer Guide {#openvino_docs_MO_DG_Deep_Learning_Model_Optimizer_DevGuide}

Model Optimizer is a cross-platform command-line tool that facilitates the transition between the training and deployment environment, performs static model analysis, and adjusts deep learning models for optimal execution on end-point target devices.

Model Optimizer process assumes you have a network model trained using a supported deep learning framework. The scheme below illustrates the typical workflow for deploying a trained deep learning model:

![](img/workflow_steps.png)

Inference Engine enables _deploying_ your network model trained with any of supported deep learning frameworks: Caffe\*, TensorFlow\*, Kaldi\*, MXNet\* or converted to the ONNX\* format. To perform the inference, the Inference Engine does not operate with the original model, but with its Intermediate Representation (IR), which is optimized for execution on end-point target devices. To generate an IR for your trained model, the Model Optimizer tool is used.

The IR is a pair of files describing the model: 

*  <code>.xml</code> - Describes the network topology

*  <code>.bin</code> - Contains the weights and biases binary data.

> **TIP**: You also can work with the Model Optimizer inside the OpenVINO™ [Deep Learning Workbench](@ref workbench_docs_Workbench_DG_Introduction) (DL Workbench).
> [DL Workbench](@ref workbench_docs_Workbench_DG_Introduction) is a platform built upon OpenVINO™ and provides a web-based graphical environment that enables you to optimize, fine-tune, analyze, visualize, and compare 
> performance of deep learning models on various Intel® architecture
> configurations. In the DL Workbench, you can use most of OpenVINO™ toolkit components.
> <br>
> Proceed to an [easy installation from Docker](@ref workbench_docs_Workbench_DG_Install_from_Docker_Hub) to get started.

**Typical Next Step:** [Preparing and Optimizing your Trained Model with Model Optimizer](prepare_model/Prepare_Trained_Model.md)

## Videos 1

\htmlonly
<iframe width="560" height="315" src="https://www.youtube.com/embed/Kl1ptVb7aI8" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<iframe width="560" height="315" src="https://www.youtube.com/embed/BBt1rseDcy0" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<iframe width="560" height="315" src="https://www.youtube.com/embed/RF8ypHyiKrY" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
\endhtmlonly

## Videos 2

\htmlonly
<iframe width="260" src="https://www.youtube.com/embed/Kl1ptVb7aI8" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<iframe width="260" src="https://www.youtube.com/embed/BBt1rseDcy0" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<iframe width="260" src="https://www.youtube.com/embed/RF8ypHyiKrY" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
\endhtmlonly

## Video: Model Optimizer Concept

[![](https://img.youtube.com/vi/Kl1ptVb7aI8/0.jpg)](https://www.youtube.com/watch?v=Kl1ptVb7aI8)
\htmlonly
<iframe width="560" height="315" src="https://www.youtube.com/embed/Kl1ptVb7aI8" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
\endhtmlonly

## Video: Model Optimizer Basic Operation
[![](https://img.youtube.com/vi/BBt1rseDcy0/0.jpg)](https://www.youtube.com/watch?v=BBt1rseDcy0)
\htmlonly
<iframe width="560" height="315" src="https://www.youtube.com/embed/BBt1rseDcy0" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
\endhtmlonly

## Video: Choosing the Right Precision
[![](https://img.youtube.com/vi/RF8ypHyiKrY/0.jpg)](https://www.youtube.com/watch?v=RF8ypHyiKrY)
\htmlonly
<iframe width="560" height="315" src="https://www.youtube.com/embed/RF8ypHyiKrY" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
\endhtmlonly
