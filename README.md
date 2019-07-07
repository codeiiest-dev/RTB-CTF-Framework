# RootTheBox CTF Framework

A CTF framework(in flask) for HackTheBox style machines. 

## Features

* Flask Blueprints
* Easily deployable on Heroku.
* User Registration, account management, Forgot password
* Hash submission (currently 2 hashes: user and root)
* Real time scoreboard tracking
* A page to show relevant details about the machine such as name, IP, OS, points and difficulty level. 

## How To Use

Using this as simple as anything. Just configure your CTF settings in `config.py`.

#### Creating database instance file

Locally or with docker,

	$ source venv/bin/activate
	$ python3 # open python interpreter
	>>> from FlaskRTBCTF import db, create_app
	>>> db.create_all(app=create_app())

For Heroku, 

	$ heroku run python
	>>> from FlaskRTBCTF import db, create_app
	>>> db.create_all(app=create_app())

## To-do

- [ ] isAdmin column in User table and Admin views (priority)
- [ ] Support for more hashes
- [ ] Testing Password reset functionality
- [ ] More info for `home.html`
- [ ] Need to implement `account.html` (not a priority)

<hr/>

- [x] Use Flask Blueprinsts
- [x] Finalize black theme?
- [x] Error messages not appearing in `/submit`
- [x] Implement `machine.html` to server a page where one can download/serve machines
- [x] Add basic info and stuff to `layout.html`
- [x] User is able to submit hash multiple times and keep increasing score, so need to implement limitations


## Screenshots

<img src="screenshots/home_ss.png" width=400 />
<img src="screenshots/home_ss.png" width=400 />
<img src="screenshots/home_ss.png" width=400 />
