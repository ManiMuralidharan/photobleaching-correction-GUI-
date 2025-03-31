The practical steps of using this photobleaching correction GUI in MATLAB.

1. Save the Code as a MATLAB Function:

Open MATLAB.
Create a new script (File > New > Script).
Copy and paste the entire code into the script.
Save the script as photobleaching_correction_GUI.m. Make sure the filename matches the function name.
2. Run the Function:

In the MATLAB command window, type:
Matlab

photobleaching_correction_GUI
Press Enter. This will launch the photobleaching correction GUI.
3. Understanding the GUI:

Load Image Button:
Click this to select a multi-frame TIFF image (.tif or .tiff).
Select Background ROI Button:
Click this to draw a rectangle ROI on the displayed image. This ROI should represent a region where you expect minimal changes in intensity over time (i.e., the background).
Preview Background Subtraction Button:
Click this to see the image with the background intensity subtracted.
Apply Correction Button:
Click this to apply the photobleaching correction.
Save Image Button:
Click this to save the corrected image stack as a TIFF file.
Frame Slider:
Use this to navigate through the frames of the loaded image.
Method Menu (Dropdown):
Select the correction method: "Single Exp" (single exponential) or "Double Exp" (double exponential).
Image Display Axes:
Displays the loaded, background-subtracted, or corrected image frames.
Intensity Graph Axes:
Displays the mean intensity of the image frames before and after correction.
4. Step-by-Step Usage:

Load the Image:
Click the "Load Image" button.
Select your multi-frame TIFF file.
The first frame of the image will appear in the image display axes.
Select the Background ROI:
Click the "Select Background ROI" button.
Draw a rectangle around a region that represents the background.
The code will calculate the background intensity for each frame.
Preview Background Subtraction (Optional but Recommended):
Click the "Preview Background Subtraction" button.
Observe the image in the display axes. This step helps to check if the background ROI was selected correctly.
Apply Photobleaching Correction:
Select the desired correction method from the dropdown menu ("Single Exp" or "Double Exp").
Click the "Apply Correction" button.
The code will apply the correction, and the corrected image will be displayed.
The intensity graph will display the mean intensity before and after correction.
Navigate Frames:
Use the frame slider to navigate through the frames of the corrected image.
View the Intensity Graph:
Observe the intensity graph to see the effect of the photobleaching correction.
Save the Corrected Image:
Click the "Save Image" button.
Choose a filename and location to save the corrected image stack.
Close the GUI:
Close the figure window when you are finished.
Key Considerations:

Background ROI Selection: The accuracy of the photobleaching correction depends heavily on the quality of the background ROI selection. Make sure to choose a region that represents the background accurately.
Correction Method: Experiment with both single and double exponential correction methods to see which one provides the best results for your data.
Image Format: The code is designed to work with multi-frame TIFF images.
Error Handling: The code includes error handling to catch potential issues, such as loading invalid files or selecting invalid ROIs.
Computational Intensity: The bleach correction can be computationally intensive for very large image stacks. Be patient during processing.
