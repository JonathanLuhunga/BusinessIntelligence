Business Intelligence Reports
=============================


.. BI:: Now that we have our basic skeleton,
          let's document the project.
          As you might have guessed from the name,
          we'll be documenting a basic web crawler.

For this project,
we'll have the following pages:

* Index Page
* Support
* Installation
* Cookbook
* Command Line Options
* API

Let's go over the concepts we'll cover,
and then we can talk more about the pages to create.

Serveur Centre de rapports
**************************

A lot of these RST syntax examples are covered in the Sphinx :ref:`sphinx:rst-primer`.

.. index::
   pair: Syntax; Hyperlink

But
-----

Every Sphinx document has multiple level of headings.
Section headers are created by underlining 
the section title with a punctuation character, at least
as long as the text.

They give structure to the document,
which is used in navigation and in the display in all output formats.

Reporting
********

Installation documentation is really important.
Anyone who is coming to the project will need to install it.
For our example,
we are installing a basic Python script,
so it will be pretty easy.

But
-----

Include the following in your ``install.rst``, 
on the same level as ``index.rst``, properly marked up:

Analyses
************

Have some extra time left?
Check out these other cool things you can do with Sphinx.

Analyse descriptive
-------------------

The beauty of Sphinx is that it can output in multiple formats,
not just HTML.
All of those formats share the same base format though,
so you only have to change things in one place.
So you can generate a manpage for your docs::

  make man

This will place a manpage in ``_build/man``.
You can then view it with::

  man _build/man/crawler.1

Analyse prescriptive
--------------------

Some people prefer one large HTML document,
instead of having to look through multiple pages.
This is another area where Sphinx shines.
You can write your documentation in multiple files to make editing and updating easier.
Then if you want to distribute a single page HTML version::

  make singlehtml

This will combine all of your HTML pages into a single page.
Check it out by opening it in your browser::

    open _build/singlehtml/index.html

.. note:: You'll notice that it included the documents in the order
          that your :ref:`TOC Tree <toctree-syntax>` was defined.

Prise de decisions
------------------

Now it is time to move on to :doc:`step-2`.


