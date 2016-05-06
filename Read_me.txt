---------------------------------------------------------------------------
Project: Facial Interpretation for Human-Robot Interaction
---------------------------------------------------------------------------
---------------------------------------------------------------------------
In this folder you must find the following files and/or folders:

1) Datasheet.xlsx 

2) FAP_and_BAP.png 

3) Image Files(folder)

4) MiniCortexDosBoxtest(folder)

5) Results.xlsx

---------------------------------------------------------------------------
***************************************************************************
---------------------------------------------------------------------------
1) Datasheet.xlsx 

The image data collected using Visage and SHORE's program in SociBot.

a) train_35 and test_35 sheet contains 35 FAP. 
b) train_32 and test_32 sheet contains 32 FAP.
c) train_38 and test_38 sheet contains 38 FAP.
d) train_22 and test_22 sheet contains 22 FAP.

FAP: Facial Animation Parameters (of Visage).

---------------------------------------------------------------------------
***************************************************************************
---------------------------------------------------------------------------
2) FAP_and_BAP.png 

Image that shows face and body animation parameters of Visage software.

---------------------------------------------------------------------------
***************************************************************************
---------------------------------------------------------------------------
3) Image Files

Folder that contains images from CK+ databse. These images were used to obtain 
Visage and SHORE data for training and testing neural network.

Emotion     Total Subjects      No. used for training  No. used for testing
-------     ---------------     ---------------------  --------------------
Angry     - 	45 			25			20
Contempt  - 	19			11			08		
Disgust   - 	59			40			19
Fear      - 	25			15			10
Happy     - 	67			39			30	
Sadness   - 	28			18			10
Surprised - 	82			50			32
Neutral   - 	43			25			18

---------------------------------------------------------------------------
***************************************************************************
---------------------------------------------------------------------------
4) MiniCortexDosBoxtest (folder) 

This folder contains:

RunDosBoxCortex.bat: the file to load and run the ANN program.
RBFLEARN.CTX: The neural network ctx file used for training and testing.

Train Files: train_a, train_b, .... to train_t
Test Files: test_a, test_b,....to test_t

On loading 'train_a' file for training the neural network, the 'test_a' file
must loaded for testing the same network. Similarly for the remaining.
(train_b and test_b, .....train_t and test_t)

How to run the program:

a) Double click on RunDosBoxCortex.bat
b) Click on load
c) Select RBFLEARN.CTX
d) Click on Edit to access the code
e) Make changes to variables if required. And, tpset to change training and testing files.
   esc + s --> to save the changes. esc + q --> to exit the code window.
f) Click on RUN.
g) Click on Learn.
h) Press esc when Nb errors reaches zero.
i) Click on test.
 

train and test text files:

            train_a,  train_e,  train_i,  train_m ---> 4 Output (Angry, Happy, Sad, Surprised) 
            train_b,  train_f,  train_j,  train_n ---> 6 Output (Angry, Disgust, Fear, Happy, Sad, Surprised)
            train_c,  train_g,  train_k,  train_o ---> 7 Output (Angry, Disgust, Fear, Happy, Sad, Surprised, Neutral)
            train_d,  train_h,  train_l,  train_p ---> 8 Output (Angry, Disgust, Fear, Happy, Sad, Surprised, Neutral, Contempt)
            -------------------------------------
No of FAP =   70,        64,       74,      44

The result files' suffix letters correspond to the train and test files used.
i.e,. ( train_a an test_a --> result_a)

---------------------------------------------------------------------------
***************************************************************************
---------------------------------------------------------------------------
5) Results.xlsx

The excel sheet contains the test results.

4 Expressions:
Test results of Angry, Happy, Sad, and Surprised test data.

6 Expressions:
Test results of Angry, Disgust, Fear, Happy, Sad, and Surprised test data.

Basic 6 + Neutral:
Test results of Angry, Disgust, Fear, Happy, Sad, Surprised, and Neytral test data.
---------------------------------------------------------------------------
***************************************************************************
---------------------------------------------------------------------------
End