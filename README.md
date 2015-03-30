Heroku buildpack: MultiMarkdown
==========================

Run a static web site from [MultiMarkdown](http://fletcherpenney.net/multimarkdown/) files bult using [MultiMarkdown-4](https://github.com/fletcher/MultiMarkdown-4).

1. Create an `index.md` file:

        echo "# hello, world" > index.md

2. Create a git repo containing the file:

        git init
        git add index.md
        git commit -m init

3. Create an app on Heroku:

        heroku create -s cedar-14 --buildpack https://github.com/npalmius/heroku-buildpack-multimarkdown.git

4. Push the repo to Heroku:

        git push heroku master

5. Open your web app:

        heroku open

