# Data-binding in AngularJS

This is the presentation for a talk I gave on data-binding in AngularJS.

## Building

This talk uses [Sass](http://sass-lang.com/) for styles, so make
sure you have that installed:

    $ gem install sass

Then compile (it's already compiled in the repository, so you can skip
this step if you don't need to modify the styles).

    $ sass css/style.scss css/style.css

Then just start a web server:

    $ python -m SimpleHTTPServer

The talk will be available at [http://localhost:8000/index.html](http://localhost:8000/index.html).
(All of the necessary Javascript libraries are included wholesale
in this repository because I wasn't sure if I would have connectivity
on site).

## About

One fun thing about this presentation is that the example code
that you see in it is also executed. This ensures that the example
code is exactly the same as the code being executed, so if you change
the code the examples stay up to date, and vice versa.

This is accomplised via the `talk-example` directive, which should be
applied to `<script />` tags. Its effect is to create a `<pre />`
element with the same contents of the original script (applying
[google-code-prettify](https://code.google.com/p/google-code-prettify/)
to the resulting code, for prettiness).  Because the original code
was in a `<script />` tag, the code itself is executed at load time.
Check it out in `js/talk.js`.
