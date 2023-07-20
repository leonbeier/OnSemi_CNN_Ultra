# OnSemi_CNN

# Training:
Open the Tensorflow_Training.ipynb file in Google Colab to train you own neural network.
New trained data can be put into the Libraries/Data_Package.vhdp file.
The parameters of the net can be changed in the Libraries/CNN_Config.vhdp file.
The CNN structure can be changed in the CNN.vhdp file.

# Excecution:
Compile the design, add the IAS Camera Extension to your Core MAX10 Ultra and use the AR0830 Camera. Then connect an HDMI monitor (most monitors should work, but some have problems with the 480p Output). Open the Serial Monitor in the VHDPlus IDE with 19200 Baud. Then you can hold the camera over a handwritten number (idealy big and written with a big black pen on white paper). You should see the white number with black surrounding in the HDMI monitor. If there is noise and it is too dark or the number is not visible and it is to bright, you can set a number between 0 and 1000 for the brightness (200-500 should work in most cases) by writing the number in the serial monitor and clicking on send. In the serial monitor you should then see the prediction and the probability that the number is correctly detected.