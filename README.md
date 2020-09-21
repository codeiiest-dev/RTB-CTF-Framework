# RootTheBox CTF Framework (CodeIIEST fork)


A fast, efficient and lightweight (~100 KB) Capture The Flag framework (in Flask) inspired by the [HackTheBox](https://hackthebox.eu/) platform.

The 100 second elevator-pitch is that: A Capture The Flag framework; one that is fast yet feature packed, efficient thus scalable, lightweight (insert some more pro developer adjectives) and customizable to your organization's brand while not emptying your bank A/C.


**Want to see it in action?**

   A live demo of the app is available at: <https://rtblivedemo.herokuapp.com/>.

   You can login and mess around as the admin user `admin:admin` (i.e. username:password combinations) or register your own.

## Build locally

### Please see [INSTALLATION.md](.github/INSTALLATION.md).

## Host a customized CTF with Heroku for free in under a minute

1. Sign up on [Heroku](https://heroku.com), if you haven't already and click on the below "Deploy to Heroku" button.

    [![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

2. Give your application an awesome name and _optionally_ specify mail environment variables.

    > Note: A psuedo-random password for the **admin** user would be created and set in the config variable `ADMIN_PASS`. On Heroku, you can reveal this password from your application's dashboard settings. Same for the Flask application's `SECRET_KEY`.

3. Open your newly deployed application in the browser, you'll be redirected to login as the `admin` user and do so.

4. Finally, you'll want to `/setup` the CTF Settings and,

#### Yay! Now you have a customized instance of the RTB-CTF-Framework live on Heroku. 🎉

> Bonus: You can manage the database CRUD operations from admin views GUI; change machine settings, issue notifications to users, etc.

## Inspiration

The main purpose of this project is to serve as a scoring engine and CTF manager. One that is packed with features, can handle enterprise/global level traffic on a scalable yet free heroku's dyno.

[CTFd](https://github.com/ctfd/ctfd) is one of the most popular CTF framework and we have used it for multiple engagements and will surely use it again. But at the same time, CTFd is heavy (~22.2 mb) (it gives poor performance even on a $49/mo heroku dyno) and not everyone has $$$ to spend on cloud, especially students (like us). So, that's where RTB-CTF-Framework (~100 KB) comes in.

## Contributing

Please refer to [CONTRIBUTING.md](.github/CONTRIBUTING.md)


# License

This project is available under a dual license: a commercial one suitable for closed source projects and a A-GPL license that can be used in open source software.

Depending on your needs, you must choose one of them and follow its policies. A detail of the policies and agreements for each license type are available in the [LICENSE.COMMERCIAL](LICENSE.COMMERCIAL) and [LICENSE.AGPL](LICENSE.AGPL) files.


## Big thanks to abs0lut3pwn4g3 for the amazing framework