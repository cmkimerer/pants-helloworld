# Pants Hello World

The goal of this repo is to provide a "Hello World" introduction to [pants](https://github.com/pantsbuild/pants).
A ton of functionality is actually missing from pants as whole, but could
be easily added to this base system.

Disclaimer: Part of what is in the repo may be unnecessary. I tried to cull
as much as a could from the [commons](https://github.com/twitter/commons) and [pants](https://github.com/pantsbuild/pants)
repos, and I may have failed at some parts. If you notice things that could
be stripped out of here to make this even more concise, please submit a pull request.

#### Current functionality includes
* Running Java Applications
* Running Python Applications
* Running Scala Applications

#### So how do I use this?
You must first have installed [sbt](http://www.scala-sbt.org/).  There may be some way to do this as part of 
the repo, but I couldn't figure out how.

I used a virtualenv for the pants installation.  And I did the following for it:

    $ virtualenv somedir --no-site-packages
    $ source somedir/bin/activate
    $ pip install pip install pantsbuild.pants --allow-external elementtree --allow-unverified elementtree    

If you want to run any of the HelloWorld commands you can do the following

    pants goal run src/java/com/example:hello-world-java-run
    pants goal run src/python/com/example:hello-world-python-run
    pants goal run src/scala/com/example:hello-world-scala-run

#### Is this useful?
Perhaps, it was useful for me in terms of teaching me how to get pants running
outside of the scope of [commons](https://github.com/twitter/commons) and [pants](https://github.com/pantsbuild/pants).
You may or may not find this useful.

This is hopefully built in such a way that you could remove all the files under 
src/* and put your own work there and your repo would be all setup for pants.
Note: Functionality in this repo is very limited, it may not even be worth it to use
this

#### But this doesn't support $FEATURE
Yea, it probably doesn't.  For any features I plan on adding in the future will
either be a separate branch or a fork of this repo.  Why?  Because it makes it easy
for everyone to see what steps are required to add certain functionality,
which also means it's easier for people to continue extending functionality of pants
for the features they need.

#### Misc
This works with scala version 2.10.1 instead of 2.9.3 (the default).  At some point
I'd like to actually upgrade it to something even more recent, but figured having
something working and public is better than having something broken and private.


