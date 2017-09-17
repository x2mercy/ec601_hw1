    #Some tips about how to install openCV on Mac:
    1. First you can download brew (https://brew.sh) and we could use brew to install openCV.
    2. You need to add before install openCV following these instruction:
    open terminal-enter code "brew tap homebrew/science"
    3. Install openCV:
    enter code "brew tap homebrew/science"
     Then we can see the location of openCV:
     /usr/local/Cellar/opencv/3.3.0_3
    4. Copy this path "/usr/local/Cellar/opencv/3.3.0_3/lib/python2.7/site-packages/cv2.so " to 
    "/anaconda/envs/braintumor/lib/python2.7/site-packages " in order to let python know that we 
    installed openCV.
    5. Run import cv2. 
    If there is a message which said "ImportError: numpy.core.multiarray failed to import", 
    you can reinstall numpy by adding the code "sudo pip install numpy --upgrade --ignore-installed".
    If the message which said "no module named cv2" came out, you could enter the following code to fix:
    cd /Library/Python/2.7/site-packages
    ln -s /usr/local/Cellar/opencv/3.3.0_3/lib/python2.7/site-packages/cv.py cv.py 
    sudo ln -s /usr/local/Cellar/opencv/3.3.0_3/lib/python2.7/site-packages/cv2.so cv2.so
    
