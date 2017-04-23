
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

File: machine/calc_correlation.py

File "machine/calc_correlation.py", line 40
    print "Usage: python calc_correlation.py <data file.py>"
SyntaxError: Missing parentheses in call to 'print'
Solution: Python 2 vs 3 problem, need to add parentheses to the print statements at line 40, 46, and 52.

// -------------------------------------------------------

File: machine/ml_main.py 
SyntaxError: Missing parentheses in call to 'print'
Solution: Python 2 vs 3 problem, need to add parentheses to the print statements at line 41, 47, 51, 53, and 55.

// -------------------------------------------------------

File: Multiprocessing/gen_rand.py
SyntaxError: Missing parentheses in call to 'print'
Solution: Python 2 vs 3 problem, need to add parentheses to the print statements at line 9.

// -------------------------------------------------------

File: Pandas/obesity.py
SyntaxError: Missing parentheses in call to 'print'
Solution: Python 2 vs 3 problem, need to add parentheses to the print statements at line 5, and 28.

// -------------------------------------------------------

File: Pandas/pandas_movie.py
SyntaxError: Missing parentheses in call to 'print'
Solution: Python 2 vs 3 problem, need to add parentheses to the print statements at numerous lines.

UnicodeDecodeError: 'utf-8' codec can't decode byte 0xe9 in position 3: invalid continuation byte
Solution: adds "encoding = 'ISO-8859-1'" to read_csv at line 12.
  - http://stackoverflow.com/questions/18171739/unicodedecodeerror-when-reading-csv-file-in-pandas-with-python

pandas_movie.py:19: FutureWarning: order is deprecated, use sort_values(...)
pandas_movie.py:27: FutureWarning: order is deprecated, use sort_values(...)
pandas_movie.py:47: FutureWarning: by argument to sort_index is deprecated, pls use .sort_values(by=...)
pandas_movie.py:62: FutureWarning: sort is deprecated, use sort_values(inplace=True) for INPLACE sorting

// -------------------------------------------------------

File: rpi/webapp_bootstrap.py
TypeError: a bytes-like object is required, not 'str'
Solution: Python 2 vs 3 problem, need to add ".decode()" to line 19.
  - http://stackoverflow.com/questions/29643544/python-a-bytes-like-object-is-required-not-str

// -------------------------------------------------------

File: rpi/webapp.py
TypeError: a bytes-like object is required, not 'str'
Solution: Python 2 vs 3 problem, need to add ".decode()" to line 19.
  - http://stackoverflow.com/questions/29643544/python-a-bytes-like-object-is-required-not-str

// -------------------------------------------------------
// -------------------------------------------------------
// -------------------------------------------------------
