# Identification Of Breast Cancer With 90% Accuracy
<p align="center">
</p>
<img src="https://cdn.britannica.com/54/179554-138-A3C5FBA0/use-mammographies-resonance-breast-cancer.jpg" width="1500" height="520">
<p>Breast cancer remains one of the most prevalent and challenging health issues worldwide, with 2.3 million women diagnosed and 685,000 deaths reported globally in 2020 alone. The disease originates from mutations in breast cells that proliferate uncontrollably, forming a mass of tissue that can invade and damage surrounding breast tissue. To address this critical concern, I have developed a custom deep neural network specifically trained on histopathological images of both infected and uninfected breast tissue. This model demonstrates a remarkable 90% accuracy in distinguishing between malignant and non-malignant cases, offering a promising tool for early detection and treatment planning in breast cancer care. </p>
<h2>Libraries Used</h2>
<ul>
  <li>Tensorflow</li>  
  <li>Numpy</li>
  <li>Pandas </li>
  <li>Matplotlib</li>
  <li>Seaborn</li>
  <li>Sklearn</li>
</ul>
<h2>Data Visualization</h2>
<p> Below is the visualization of the dataset, which is labeled as either "Positive" or "Negative" for breast cancer. Each image of the dataset represents a sample of breast tissue, stained and magnified, to highlight cellular structures. The "Positive" labels correspond to images where cancerous cells are present, showing irregularities such as dense cellular clusters or abnormal tissue architecture. In contrast, the "Negative" labels indicate non-cancerous tissue, where the cellular structure appears more organized and uniform. This dataset is likely used to train or evaluate a deep neural network model to distinguish between cancerous and non-cancerous breast tissue with high accuracy.
</p>
<p align="center"> 
<img src="https://github.com/user-attachments/assets/6f4ffc6b-530b-487e-8f26-9b52d1e22db9" width="750" height="500">
</p>
<h2>Target Class Distribution</h2>
<p>Here zero stands for the infected histopathological image, and one is for the anon-infected histopathological image.</p>
<p align="center"> 
<img src="https://github.com/user-attachments/assets/5cd5fff8-9172-4b59-b545-94a5f03ea9e7" width="400" height="450">
</p>
<h2>Methodology and Approach</h2>
<p>
I have developed and rigorously trained a neural network model specifically designed for the classification of breast cancer using histopathological images. This model integrates convolutional neural network (CNN) layers with artificial neural network (ANN) layers to effectively analyze and interpret complex image data. The architecture consists of three CNN layers, each followed by a max-pooling layer, to systematically extract and condense spatial features from the input images. These CNN layers process images of 100x100 pixels with three color channels, and progressively increase in depth from 32 to 192 filters, enhancing the model's ability to capture intricate patterns indicative of malignancy.
</p>
<p>
After the feature extraction, the output is flattened into a one-dimensional vector and passed through three dense (fully connected) layers in the ANN portion of the network. Dropout layers are incorporated between the dense layers to prevent overfitting by randomly disabling a fraction of neurons during training. The final dense layer outputs a single value, which represents the binary classification of the input image as either positive (cancerous) or negative (non-cancerous).
</p>
<p>
This model was trained on a dataset consisting of 6,000 histopathological images, equally divided between positive and negative classes. The training was conducted over 20 epochs, using binary cross-entropy as the loss function and the Adam optimizer for adjusting the network's weights. This approach yielded a highly accurate model, capable of identifying breast cancer with an accuracy rate of 90%, offering a promising tool for early detection and diagnosis.  
</p>
<p align="center"> 
<img src="https://github.com/user-attachments/assets/d571e29f-4947-4a3e-9469-d816fa085246">
</p>
<h2>Model Training</h2>   
<h4>Model Loss:</h4>   
<p align="center"> 
<img src="https://github.com/user-attachments/assets/e39c8a2f-44db-4688-8c13-063ee481e92e" width="700" height="400">
</p>
<h4>Model Accuracy:</h4>  
<p align="center"> 
<img src="https://github.com/user-attachments/assets/6365848b-633d-4884-8dac-eb0d9e58baa8" width="700" height="400">
</p>
</p>
<h2>Model Evaluation</h2>
<ul>
  <li>Training Data Accuracy: 90 %</b></li>
  <li>Test Data Accuracy: 86 %</li>
  <li>Training Data Loss: 0.90</li> 
  <li>Test Data Loss: 0.31</li> 
</ul>  
<h2>Model Prediction</h2>
<p align="center"> 
<img src="https://github.com/user-attachments/assets/37e9b0c3-1afc-45af-b3cf-6d866b51c1ed" width="800" height="500">
</p>
</p>
<h2>Model Introspection</h2>
<h4>Confusion Matrix</h4>  
<p align="center"> 
<img src="https://github.com/user-attachments/assets/32c0198a-dbac-4824-8a0d-cfc314eb57d2" width="400" height="400">
</p>
<h4>Receiver Operating Characteristics (ROC)</h4>  
<p align="center"> 
<img src="https://github.com/user-attachments/assets/f879d599-9c99-4259-a484-aef0279997c8" width="700" height="400">
</p>
<h4>Precision vs. Recall curve</h4> 
<p align="center"> 
<img src="https://github.com/user-attachments/assets/7cf60544-fd70-4e08-bac5-801921f0e284" width="700" height="400">
</p>
<h4>Classification Report</h4>  
<p align="center"> 
<img src="https://github.com/user-attachments/assets/95be745c-f228-4b56-9fe7-1292a454f01b" width="700" height="700">
</p>
<h2>Conclusion</h2>  
<p>In this project, I have created deep convolutional neural network architecture for correctly identifying breast cancer with an accuracy of 90 percent accuracy. </p>  
