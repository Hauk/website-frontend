# Contributing #
So you are ready to battle with code? Good.

---

## Technologies ##
After a long debate we decided to not use plain Javascript.
Why? Because trying to expand the codebase is pretty difficult after a while.
Instead we decided to use [Dart](http://dartlang.org).
If you look at the code you will see that the syntax is very similar to languages such as Java or C.

The default installation procedure is kinda weird,
so we made a wiki page [Dart Installation](https://github.com/redbrick/website-frontend/wiki/Dart-Installation)

---

## Installation ##
Make sure you have Dart installed

1. Clone the git repo
2. In the repo root run `pub get`. This will install all the necessary dependencies
3. To quickly test everything run `pub serve`. This will create a HTTP server running on port `8080`. Run `pub help` to get information on how to change the port

---

## Issues ##
To make sure issues are descriptive as possible, please use the following issue template:
```
Name: Short but descriptive, no more than 6 words

In Issue:
  Description:  Give a more detailed explanation of an issue or suggestion.
                Be precise, but don't write a novel

  Steps to reproduce: If you are filing an bug, list the steps necessary to replicate
                      the bug using. eg:
                        1. Go to #/about
                        2. Click on `Home`
                        3. You get redirected to #/home instead of /

  Optional: Include an image of the issue or suggestion as it is
            found on some other page. If possible also include links
```
After an issue is filed a maintainer will look at it and give it appropriate labels and assign it to a milestone.
Please do not be offended if a suggested feature is turned down,
there might be a valid reason for it, but if you feel that the
maintainers are too lazy to implement it, do it yourself.

---

## Forking, Branches and Commits ##
Since we can't just allow everybody committing to the main repo,
if you want to make changes, please create a fork of the repo.
In there, make your own branch. When it comes to branch formats,
use this standard:

* `feature/FEATURE_NAME`: All new features
* `bugfix/BUGFIX_NAME`: Bugfixes

That way when you file a pull request we know exactly at first glance what the PR is.

Please merge main project `master` into your fork often to make sure there are no merge issues. When you start working on an issue make sure you state that you are doing it, otherwise you might have others doing the same thing.

When you are adding a commit of your change, it is better to have more smaller commits than large big one.
Preferably a commit per file or commit per change. That way if something goes wrong,
a single commit can be reverted without breaking much.
Please do not speak in first person `"I added ___"` but rather `"Added ___"`.
In commits also make sure you reference the file you have changed and its section.
This allows to see the what files the commits changed without reading the files themselves

---

## Pull Requests ##
When you are done with a feature or a bugfix,
you will have to file a pull requests with will integrate your change back to `master`. Your code will be peered reviewed by the repo maintainers. You might be asked to change certain things, and the pull request will not be merged until all issues are resolved.

---

## Testing ##
While this doesn't apply that much to frontend, as there will not be that much scripting (hopefully),
all functions must have unit tests written (and preferably also integration).
We will be using a Continous Integration platform to make sure all tests pass before merging into master.
That way we can make sure that things don't break down the line as we change things down the line.
Your Pull Request will not be merged if it doesn't pass all the test (just because you don't have tests doesn't mean they would pass)

---
