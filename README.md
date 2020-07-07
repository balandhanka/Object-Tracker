# Object-Tracker
## USAGE
### python `track.py --video video/video.mp4`
## Steps:-
   + defined the upper and lower boundaries for a color to be considered "blue".
   + load the video.
   + grab the current frame.
   + check to see if we have reached the end of the video.
   + determine which pixels fall within the blue boundaries and then blur the binary image.
   + find contours in the image.
   + check to see if any contours were found.
   + sort the contours and find the largest one -- we will assume this contour correspondes to the area of object in blue colour.
   + compute the (rotated) bounding box around then contour and then draw it.
   + show the frame and the binary image.
   + if your machine is fast, it may display the frames in what appears to be 'fast forward' since more than 32frames per second are being displayed -- a simple hack is just to sleep for a tiny bit in between frames.
   + cleanup the camera and close any open windows.
