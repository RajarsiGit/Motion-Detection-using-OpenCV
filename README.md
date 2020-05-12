# Basic Motion Detection
 
 This code is used to detect motions of objects in an environment and also count the number of objects. This is done using OpenCV.
 
 First the video is splits and then the frames are read one by one. We gray out the frames, blur the frames using some preset values and then apply threshold to separate the moving pixels from the stagnent pixels. This data is now taken and a contour is made from it. The bounds of the contour form the bounds of the green box, indicating motion.
 Initial frame is taken to be the reference frame, and OpenCV calculates the difference in the matrix data. Any change in the matrix data tells us that there is movement and those areas are marked.
