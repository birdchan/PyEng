
// just make sure the python version is 3.x, not 2.7
(py3k) Brians-MacBook-Pro:PyEng brian$ python --version
Python 3.6.0 :: Anaconda 4.3.1 (x86_64)

// -------------------------------------------------------

File: Image_Video/blur.py 

ModuleNotFoundError: No module named 'cv2'
Probably cause: cv2 package is missing
Solution: install opencv, see Readme_opencv.txt

cv2.waitKey(0) doesn't release the terminal
I had to do Ctrl-Z, then look up the pid and kill it.

// -------------------------------------------------------

File: Image_Video/color_test.py

ModuleNotFoundError: No module named 'SimpleCV'
Probably cause: SimpleCV package is missing
Solution: Follow the numerous commands at this URL to install SimpleCV
  - https://github.com/sightmachine/SimpleCV

// -------------------------------------------------------

File: Image_Video/color_train.py

ModuleNotFoundError: No module named 'SimpleCV'
Probably cause: SimpleCV package is missing
Solution: Follow the numerous commands at this URL to install SimpleCV
  - https://github.com/sightmachine/SimpleCV

// -------------------------------------------------------

File: Image_Video/count_cards.py

  File "Image_Video/count_cards.py", line 21, in <module>
    contours, hierarchy = cv2.findContours(canny, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
ValueError: too many values to unpack (expected 2)

Probably cause: 
Solution: return 3 items: _, contours0, hierarchy
  - http://stackoverflow.com/questions/25504964/opencv-python-valueerror-too-many-values-to-unpack
  - https://github.com/opencv/opencv/blob/master/samples/python/contours.py

// -------------------------------------------------------




// -------------------------------------------------------
// -------------------------------------------------------
// -------------------------------------------------------
// sample
File: Pandas\Obesity.py
Error: XXXX

Probable cause: Library Y missing / Python 2 vs 3 problem / I dont know

