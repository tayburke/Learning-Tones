# Learning-Tones

# User Interface

User's should interact with the notebook ("LearningTones.ipynb") through this section, which is located towards the bottom of the page. 

Additional files needed for download:
1. "requirememts.txt"
2. "model_spec.txt"
3. "model.h5"
4. "model.json"

## Opening LearningTones.ipynb
First, downlowd all the files as well as the notebook into a folder or location together. Since this is a jupyter notebook, it can best be run from the termial/command prompt. If one does not have jupyter notebooks installed, they can use [google's online notebook service](https://cloud.google.com/ai-platform-notebooks/) through their google account, another IDE that is jupyter notebook compatible (ex: canopy), or by installing jupyter notebooks. The latter is the easiest and can be done through the command prompt by entering the following: 
```
pip install notebook
``` 
Once installed, either open up jupyter notebooks through the terminal by entering 
```
jupyter notebook
```
and navigating to the where "LearningTones.ipynb" is located on your disk or cd to the location where "LearningTones.ipynb" is and entering 
```
jupyter notebook LearningTones.ipynb
```
in the command prompt. Jupyter notebooks will open on a web browser page, but no fear, it does not require the internet-- it uses a port on the local host (your computer) to run on the browser page. [This website](https://jupyter-notebook-beginner-guide.readthedocs.io/en/latest/execute.html) will be helpful in getting jupyter notebooks up and running if you are facing any issues. 

Whenever I refer to "running" cells (i.e blocks of code), I just mean clicking the the little play button located at the top of the page. If you find any issues, how to navigate jupyter notebooks itself can be found [here](https://www.codecademy.com/articles/how-to-use-jupyter-notebooks).

## Importing packages and the trained classifying model
All imports that are needed are included under the import section. You will need the "requirememts.txt" file in order to install certain packages. There has been reportted issues on Windows computers installing librosa. This can be potentially solved by openening the command prompt/ terminal, write the line 
```
pip install librosa --user
```
The package should be installed properly after that. If there are any issues feel free to email me at tburke3@wellesley.edu, and we can work on getting you the necessary packages to run the file. From there, the user needs to run the "Load in the model" section. This will load in the model that was previously found to be optimal for classifying tones. Luckily, it is already saved and the user does not have to retrain it-- it just needs to be compiled! When done compiling it, it will print out details about the model. 

## Classifying audio
Finally, you are ready to start classifying your audio into the four tones of Mandarin Chinese. 

- [ ] **Create folder to hold user audio**
> You will create a folder to hold all your audio files. This just creates a folder to store the audio recordings for the  
> current session. In case you want to always be able to refer back to your learning over time, do the following: remove the 
> line shutil.rmtree(user_audio_directory) under **Create folder to hold user audio** and all the code under the section
> titled > **Delete all user recordings**. 

- [ ] **Record user's voice**

> You will be able to record your voice for 1.4 seconds. You will be prompted when to start recording and told when you are 
> done recording. 

- [ ] **Plot, playback, and prediction of user recording**

> If you are satisfied with your recording, you can have it played back to you, plotted by a waveform for visualization, and
> be given real time auditory feedback from the model by its predicting the tone and reporting the accuracy. The model itself
> has an accuracy of ~98.10% across classifying ~10,000 monosyllabic Mandarin words in 10-fold cross validation, so it is 
> pretty accurate! You can toggle between this section and the section above as many times as they like! 

- [ ] **Delete all user recordings**
> At the end, you can delete all their recordings for storage space purposes by running the last block of code.  

:+1: Have fun and good luck in learning Mandarin tones!

