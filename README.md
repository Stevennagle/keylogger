# keylogger -Project Completed

------------------------------------------------------------------
Python Key-logger based on an online tutorial at :

	https://www.youtube.com/watch?v=yvHrNlAF0Y0

==================================================================

Dependencies : 

	PyNput : 

https://pypi.org/project/pynput/

https://github.com/moses-palmer/pynput

==================================================================

1) cd pynput-master
2) python setup.py install
3) import pynput



==================================================================

Troubleshooting :


Problem #1 

Problem found running in git bash on Win64 :

	Error : 
		
		After typing python in git bash cursor moves to next line without providing default Python input prompt ">>>"

	Solution : 
		cd ~
		touch .bashrc
		<edit file with :> alias python='winpty python.exe'


==================================================================

Problem #2

	Error message : 

"...\AppData\Local\Programs\Python\Python37\lib\site-packages\pynput-1.4.2-py3.7.egg\pynput\_util\__init__.py", line 78, in inner
    if f(*args) is False:
  File "./keylogger.pyw", line 11, in on_press
    logging.info(str(key))
Message: "'s'"
Arguments: ()
..."

--	--	--	--	--	--	--	--	--	--	--	--	--	--	--	--	--	

Cause: 	
	Line : 8 -> wrong code == "... format ='%(asctime)s: %(messages)s:')"

Solution :
	Line : 8 -> right code == "... format ='%(asctime)s: %(message)s:')"

