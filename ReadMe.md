
This project uses pixel data lifted from images present in this directory, 
to test this project locally, you will need to run the csf38.html file in a browser such as chrome.

On mac you will need to run the following command in your terminal 

open -n -a "Google Chrome" --args --user-data-dir=/tmp/temp_chrome_user_data_dir http://localhost:3000/ --disable-web-security 

On windows run the following from within the directory of chrome

chrome.exe  --disable-site-isolation-trials --disable-web-security --user-data-dir="D:\temp"

These commands open an instance of chrome with disabled security, this allows the pixel data to be from a local origin. 

Once the csf38.html has loaded, it will access the wnet.js file by default and load it into the program. 
wnet is a trained diffusion model that can produce fruit-like smudges under proper guidance. 

![Alt Text](https://ditzbitz.com/fshett.gif)



There are some hotkeys to operate the model, which are as follows:

E: Detach training, this does nothing in the trained model

Space: start the network with and align the inputs to be the same as the inputs given in training (to print the training data)

Y: Hybridize the output of the network with static, just to see 

M: Provide purely the previous output as input, check for attractors

C: stop the count, and lock the image projection on a single fruit/input

T: Recume training, again, no value in trained model. 

Z: start the network and Shift data input seed to offset to 1 instead of 0 (see some diffused fruit)

3: Print out the trained network. 

R: hold to Convert the current input to a gradient. 

O: start the network with totally random inputs


