# Emotive IOT Lighting 
Emotion recognition for attention and focus vs distraction and tiredness, using TensorFlow on Raspberry Pi 3. 
Pictures captured on the Pi's camera are analyzed by TensorFlow models trained on the Kaggle fer2013 labelled facial emotional recognizion data.
This data has been well studied and characterized, and contains lables for 7 basic emotions.
The TF fer2013 model will be fed new labelled data of face pictures showing attention vs inattention.
The resulting output vectors will be analyzed using PCA to find a single vector that predicts changes in attention.

These attributes will be mapped to color changes in a small desktop lamp. Users will be able to practice better work hygiene practices by taking intelligent breaks, as cues from the lamp will generated based on their attention deltas, and calibrated using academic studies of ideal break intervals.

Additionally, the resulting output vectors will be logged in a cloud database, where user's can view their personal data using interactive web frameworks such as D3.

## Completed:

### Acquire hardware:

  Raspberry Pi 3
  
  NOIR Night Vision Camera
  
  RGB LED desktop lamp
  
  Rasberry Pi infrared reciever / transmitter 

### Hardware Config

  Set up Pi as headless SSH server
  
  Test IR camera in varying lighting conditons
  
  Test openCV face tracking
  
  Install TensorFlow, test networks
  
### Web server

  Register domain name
  
  Configure web hosting
  
  Build website template
  
  
## Next:

### Neural Network Calibration

  Find, test accurate emotional recognition model
  
  Evaluate accuracy for tired/attentive faces
  
  Acquire training images for tired/attentive faces (scrape image searches)
  
  Test against emotive model
  
  Use PCA in SKLearn to model accuracy on tired/attentive faces
  
### IR Remote

  Capture desktop RGB LED lamp color control signals from remote with RPi IR reciever board
  
  Transmit color commands to lamp from Raspberry Pi 3
  
### Capture Test Data

  Set camera to record snapshots at set intervals (as defined by the TensorFlow's throughput speed). Start with 30 seconds adjust as necessary.
  
  Compare snapshots to model output for heuristic accuracy
  
  Reiterate design
  
### Web Server

  Implement SQLite databse to record model output snapshots
  
  Add DB interface with interactive D3 analytics suite
  
  
  
  


