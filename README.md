BHRShellScriptLibrary
=====================

What is the Shell Script Library?
---------------------------------
The Script Library is a collection of useful bash scripts, which can be accessed by all SimpleSSH users. 

Everyone can contribute to the Script Library and make his scripts available for other users.


We're happy to help you, if you need assisstance adding your scripts or have problems adding them.


How to Contribute
-----------------
You can add scripts by creating a pull request to the main Script Library repository.

1. Fork BHRScriptLibrary.
2. Add your scripts to `scripts.json` by respecting the script guidelines.
3. Validate `scripts.json` with <http://jsonlint.com>
4. Press the green button in the upper left corner, review your changes and submit the pull request via `Create Pull Request`.
5. After being reviewed, your scripts will be part of the Script Library.


Script Guidelines
----------------------

All scripts are located in `scripts.json`. 
The basic structure is a an array of `Groups`, that have children. Each child is a `Command`.

Illustration:
```
[	
	Group
		[
			Command,
			Command
		],
	Group
		[
			Command,
			Command,
			Command
		]
]
```

A `Group` must have the following properties:  

* Name
* Description
* UID
* Children (Array of Commands)

A `Command` must have the following properties:

* Name
* Description
* Script
* Show Result
* Timeout (0 is no timeout)
* UID

For UID generation please use <http://www.guidgenerator.com>.



Additional Resources:
---------------
* <https://help.github.com/articles/fork-a-repo>
* <https://help.github.com/articles/creating-a-pull-request>
* <http://json.org>
* <http://jsonlint.com>



Disclaimer
----------
No guarantee is provided that the scripts will function properly on your system. Some require additional packages. No warranty for loss or corruption of any data.

Use the scripts at your own risk!