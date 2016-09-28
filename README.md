# Emotive IOT Lighting 
Emotion recognition for attention and focus vs distraction and tiredness, using TensorFlow on Raspberry Pi 3. 
Pictures captured on the Pi's camera are analyzed by TensorFlow models trained on the Kaggle fer2013 labelled facial emotional recognizion data.
This data has been well studied and characterized, and contains lables for 7 basic emotions.
The TF fer2013 model will be fed new labelled data of face pictures showing attention vs inattention.
The resulting output vectors will be analyzed using PCA to find a single vector that predicts changes in attention.

These attributes will be mapped to color changes in a small desktop lamp. Users will be able to practice better work hygiene practices by taking intelligent breaks, as cues from the lamp will generated based on their attention deltas, and calibrated using academic studies of ideal break intervals.

Additionally, the resulting output vectors will be logged in a cloud database, where user's can view their personal data using interactive web frameworks such as D3.

# Completed Tasks:

### Scope and vision:

  - [x] Action-ready conceptual diagram based on domain research

### Acquire hardware:

#### Raspberry Pi 3 and peripherals
  
  - [x] NOIR Night Vision Camera
  
  - [x] Rasberry Pi infrared reciever / transmitter 
  
#### Lighting  
  
  - [x] RGB LED desktop light

### Initial Config RPi

#### Hardware
  - [x] Set up Pi as headless SSH server
  
  - [x] Test IR camera in varying lighting conditons

  - [x] Overlock CPU to 1400 GHz, memory to 500
  
  - [x] Activate dynamic GPU / RAM allocations
  
#### Software
  
  - [x] Test openCV face tracking
  
  - [x] Install and compare TensorFlow, Caffe
  
### [x] Web server

  - [x] Register domain name
  
  - [x] Configure web hosting
  
  - [x] Build website template
  
  
# In progress:

### Neural Network Calibration

  Find, test accurate emotional recognition model
  
  Evaluate accuracy for tired/attentive faces
  
  Acquire images of tired/attentive faces for fine tuning
  
  Test against emotive model
  
  Use PCA in SKLearn to model accuracy on tired/attentive faces
  
  
# Next:  
  
### IR Remote

  Capture desktop RGB LED lamp color control signals from remote with RPi IR reciever board
  
  Transmit color commands to lamp from Raspberry Pi 3
  
### Capture Test Data

  Set camera to record snapshots at set intervals (as defined by the TensorFlow's throughput speed). Start with 30 seconds adjust as necessary.
  
  Compare snapshots to model output for heuristic accuracy
  
  Reiterate design
  
### Web Server
   
  Write network protocols to SSH of protobuf'd Python dictionary objects

  Implement redis databsse to record model output snapshots
  
  Add DB interface with interactive D3 analytics suite
  
  
# Conceptual Design
  
![alt text](https://github.com/N2ITN/RPi3_Tensor_Emotive/blob/master/images/Neural%20Emotion%20-%20Neural%20Feels.jpg)

