# Colour-Detection
It's a machine learning based project using python and pandas library
The provided code is a Python script that uses OpenCV (cv2) and pandas libraries to create a color picker application. Here's a breakdown of the code:

Import the required libraries: cv2 for image processing and pandas for data manipulation.
Specify the path for the input image ('Main.jpg') and the colors data CSV file ('colors.csv').
Define the column names for the colors data.
Read the colors data from the CSV file into a pandas DataFrame.
Load and resize the image using cv2.imread() and cv2.resize() functions, respectively.
Define variables to track mouse clicks and color values.
Create a function, get_color_name(), that finds the closest color name in the DataFrame based on the RGB values of a pixel.
Create a draw_function() that captures the mouse events, particularly a left double-click (LBUTTONDBLCLK).
Create a window named 'image' and associate the draw_function() with the mouse events in that window using cv2.namedWindow() and cv2.setMouseCallback() functions.
Enter a while loop to continuously display the image and perform color picking.
Within the loop, if a pixel has been clicked, draw a rectangle with the selected color and display the color name and RGB values on the image.
If the sum of RGB values is high (indicating a bright color), display the text in black for better visibility.
Exit the loop when the 'Esc' key is pressed.
Close all windows using cv2.destroyAllWindows().
Please note that this code assumes you have an image file named 'Main.jpg' and a CSV file named 'colors.csv' with the appropriate color data. Make sure the files exist and are accessible in the specified paths for the code to run successfully.
