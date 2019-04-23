# keylogger

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

Problem found running in git bash on Win64 :

	Error : 
		
		After typing python in git bash cursor moves to next line without providing default Python input prompt ">>>"

	Solution : 
		cd ~
		touch .bashrc
		<edit file with :> alias python='winpty python.exe'

==================================================================

