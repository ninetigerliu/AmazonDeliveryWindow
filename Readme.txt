Author: Xiao Liu
Non-commericial use open software XXX (The name has not been decided yet)

1. Files:
	* wholeFoods.ipynb is for whole foods market order
	* amazonFresh.ipynb is for amazon fresh order
2. Required package:
	* python package: selenium
		** pip install selenium
		** more details: https://pypi.org/project/selenium/
	* chromedriver.exe.
		** download at:	https://sites.google.com/a/chromium.org/chromedriver/downloads
		** put chromedriver.exe in the same folder as your ipynb files
		** add the path to this folder in your $PATH$ environment variable
3. How to use:
	* create your wholeFoods/amazonFresh order as usual
	* open jupyter notebook with wholeFoods.ipynb or amazonFresh.ipynb
	* run the first two cells, it will open a new chromebrowser
	* run cell 3 to open with amazon website
	* login in manually
	* run the other cells.
	* the last cell will keep refresh the delivery window web page. If there is a delivery window, it will beep for 20 seconds and end the code
	* please make sure the end_time > now in the last cell
4. Comments:
	* Code is tested in windows 10. Not sure about Mac
	* If you want to change the alert sound, please modify the alert_beep function.
	* The code can't not run with empty cart
	* example logs when the code is running:
		Not on schedule page, login again
		checked at 2020-04-14 20:19:17.227440 : 1
		checked at 2020-04-14 20:19:23.960706 : 2
		checked at 2020-04-14 20:19:30.539080 : 3

Have fun!

