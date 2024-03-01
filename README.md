# Guppy

[![Join the chat at https://gitter.im/guppy-mathbox/Lobby](https://badges.gitter.im/guppy-mathbox/Lobby.svg)](https://gitter.im/guppy-mathbox/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

## Synopsis

Guppy is a Javascript-based WYSIWYG editor for mathematics whose
content is stored in an XML format that makes Guppy mathematical
expressions **searchable**, **parseable**, and **renderable**.

The content of the editor can easily be extracted in a well-annotated
XML format (for searching), as well as LaTeX (for rendering), plain
text (for text applications) or a syntax tree (for
manipulating/evaluating).

## Demos

A full live demo can be found at 
[http://daniel3735928559.github.io/guppy/site](http://daniel3735928559.github.io/guppy/site)

A standalone basic demo can be found at
[http://daniel3735928559.github.io/guppy/site/examples/basic](http://daniel3735928559.github.io/guppy/site/examples/basic)

## How do I get started?

Go to the [quickstart page](https://daniel3735928559.github.io/guppy/site/doc/quickstart).

Also check the [FAQ](https://daniel3735928559.github.io/guppy/site/doc/faq.html).

## Can I see some examples?

Yes!  There are many at the [examples page](https://daniel3735928559.github.io/guppy/site/examples).  

Of particular note are: 

* [Calc](https://daniel3735928559.github.io/guppy/site/examples/calc) Numerically evaluate a guppy document.
* [Input/Output](https://daniel3735928559.github.io/guppy/site/examples/io) Import and extract editor content.
* [Mobile](https://daniel3735928559.github.io/guppy/site/examples/osk) Activate mobile keyboard functionality.
* [Style](https://daniel3735928559.github.io/guppy/site/doc/style.html) Style the editor with CSS.
* [Article](https://daniel3735928559.github.io/guppy/site/examples/article) Use guppy to render pre-existing mathematical content on a page.

## How does it work?

Editor content is stored in a specific [XML format](https://daniel3735928559.github.io/guppy/site/doc/format.html).
Editing operations then correspond to [operations on that XML](https://daniel3735928559.github.io/guppy/site/doc/internals.html).

## Can I help?

Yes!  See the [contributors page](https://daniel3735928559.github.io/guppy/site/contribute) for how, and the
[roadmap](https://daniel3735928559.github.io/guppy/site/doc/roadmap.html)
for an idea of where the project is heading.

## Build process
After making the changes in the Oppia's guppy fork, follow the below steps:
* To get started, make sure you are in the guppy directory, then run the following:
  ```
  $ cd guppy
  ```
  ```
  $ npm install --only=dev
  ```
*  To build, do
   ```
   $ npm run-script build-debug
   ```
*  To run the tests and code coverage tools, do
   ```
   $ npm test
   ```
## Verifying your changes
After adding build changes on the local guppy directory, follow the below steps to ensure the changes made are correct.
* Go to ``oppia/package.json`` file on local system.
* Find the line with ``guppy-dev``, and change the path to your local guppy fork ([Example](https://github.com/oppia/guppy/pull/9#issuecomment-1967417760)).
* Now, restart the server and manually test the guppy supported interaction thoroughly to ensure that the changes you made are not breaking any part of the code.
* After that you are all set to make a PR!
  
## License

Guppy is licensed under the [MIT License](http://opensource.org/licenses/MIT).
