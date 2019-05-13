textengine-books
====
official repo of Textengine books
----
 1. What is Textengine?
		
	Textengine is an opensource engine for interactive books and text quests.
	Now it's very raw but in future I'll improve it.
	Textengine you can get here: [Textengine repo](https://github.com/lesnoilis/textengine)

 2. How can I make my own book?
	
	Textengine engine uses standard json files. For the book to be fully operational, 3 files are needed:
		- data.json
		- info.json
		- icon.png
	The data.json file should contain a sequence of 5 groups:
		
	```json
	[
	  {
		"0": "// here is the text data"
	  },
	  {
		"0": "// here is the inscription on the 1st button"
	  },
	  {
		"0": "// here is the inscription on the 2nd button"
	  },
	  {
		"0": "// transition parameter when pressing the 1st button"
	  },
	  {
		"0": "// transition parameter when pressing the 2nd button"
	  }
	]
	```
		
	The info.json file should have 2 parameters:
		
	```
	{
		"name": "// book name",
		"author": "// author's name”
	}
	```
	>*Important:*
	> when entering text parameters in json files DO NOT use quotation marks, otherwise the application will fall with an error *“malformed json”*
	
