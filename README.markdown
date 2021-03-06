Twython - Easy Twitter utilities in Python
=========================================================================================
I wrote Twython because I found that other Python Twitter libraries weren't that up to date. Certain
things like the Search API, OAuth, etc, don't seem to be fully covered. This is my attempt at
a library that offers more coverage.

This is my first library I've ever written in Python, so there could be some stuff in here that'll
make a seasoned Python vet scratch his head, or possibly call me insane. It's open source, though,
and I'm open to anything that'll improve the library as a whole.

OAuth support is in the works, but every other part of the Twitter API should be covered. Twython
handles both Basic (HTTP) Authentication and OAuth. Older versions of Twython need Basic Auth specified -
to override this, specify 'authtype="Basic"' in your twython.setup() call.

Twython has Docstrings if you want function-by-function plays; otherwise, check the Twython Wiki or 
Twitter's API Wiki (Twython calls mirror most of the methods listed there).

Requirements
-----------------------------------------------------------------------------------------------------
Twython requires (much like Python-Twitter, because they had the right idea :D) a library called
"simplejson". You can grab it at the following link:

> http://pypi.python.org/pypi/simplejson


Example Use
-----------------------------------------------------------------------------------------------------
> import twython
>
> twitter = twython.setup(authtype="Basic", username="example", password="example")
> twitter.updateStatus("See how easy this was?")


Twython 3k
-----------------------------------------------------------------------------------------------------
There's an experimental version of Twython that's made for Python 3k. This is currently not guaranteed
to work, but it's provided so that others can grab it and hack on it. If you choose to try it out,
be aware of this.


Questions, Comments, etc?
-----------------------------------------------------------------------------------------------------
My hope is that Twython is so simple that you'd never *have* to ask any questions, but if
you feel the need to contact me for this (or other) reasons, you can hit me up 
at ryan@venodesigns.net.

Twython is released under an MIT License - see the LICENSE file for more information.
