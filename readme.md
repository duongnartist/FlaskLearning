# Flash Learning
## Table of contents
- [Video Courses](https://www.youtube.com/watch?v=MwZwr5Tvyxo&list=PL-osiE80TeTs4UjLw5MM6OjgkjFeUxCYH)
- [Day 1 Installing, Coding and  Running](#day-1-installing-coding-and-running)
## Day 1 Installing, Coding and Running
1. Install Flask
	```bash
	pip3 install flask
	```
2. Create a sample code
	```python
	from flask import Flask
	app = Flask(__name__)

	@app.route('/')
	def hello():
		return '<h1>:) Hello how are you?</h1>'

	if __name__ == '__main__':
		app.run(debug=True)
	```
3. Run this code
	- In `debug` mode, you don't need to restart by commandline to run new code.
	- You can run this code by python in `debug` mode by a condition.
	```python
	if __name__ == '__main__':
		app.run(debug=True)
	```
	- Run code by `flask`
	```bash
	export FLASK_APP=flaskblog.py
	export FLASH_DEBUG=1
	flash run
	```
	- Now you can open browser to access this web app.