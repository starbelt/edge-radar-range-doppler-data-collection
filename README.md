# Range doppler plots, CSV and Processed plots.

In order to get Range Doppler Plots, data was collected and processed through multiple scripts in order to obtain results for how the radar tracks a cubesat. The process to collecting this data is described below. 

## Run Range_Doppler_plot_withcsv.py

outputs .npy and config.npy
change the csv file name every time just make sure the file name ends in time.

## Ran Range_Doppler_processing.py

This Gives a visual of what processed data should Look like. 

Change f to the name of your .npy file make sure it is in the same folder as the Range Doppler script. 

## Then run batch_processing.py

change f to the name of your.npy file make sure it is in the same folder, change the output directory name, this will be where all the processed data goes. 

make sure to delete the prior .npy files and csv files and add the new ones within the folder running the code.

change the .csv file to be saved_radar_data_time.csv  and make sure the output file says something about the distrance

# Starting Experiment

measured 10 meters in 1 meter incriments away from radar

ran Range_Doppler_plot_withcsv.py for machine learning algorithm and for the processing script first. Then Ran Range_Doppler_processing.py to see it live and then batch_processing.py for cfar, mti, and combined processed data.


# Range doppler sattelite model on car

speed of car without sattelite model

 1.92 m/s going 3 meters
 1.987 m/s going 3 meters
 1.82 m/s going 4 meters
 1.82 m/s going 4 meters

 average speed = 1.89 m/s

 speed of car with sattelite model

 1.163 m/s going 3 meters
 1.676 m/s going 3 meters
 1.45 m/s going 4 meters
 1.24 m/s going 4 meters

 Average speed is 1.38 m/s 

With this knowlege the car was driven to and from the radar in the lab with and without the sattelite at different distances to record data and output a csv file. this and the .npy and config.npy files were run in the Batch Processing script to collect frames and various post processed data. 

# Data Collection in Mocap Room

This experiment was then repeated in the Motion Capture room in order to collect truth data with Motive. For this experiment the antenna was also put on a box with the dots glued on all pieces in the experiment for the motion capture room in order to see where the antenna, edge radar, and car with the cube-sat replica was. There was 4 runs in the motion capture room. The same batch processing script was used and the plot.py script was used to plot the truth data. 
