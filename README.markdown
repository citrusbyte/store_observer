StoreObserver
=============

Automatically expire cached fragments in Ruby on Rails based on the state of the models involved.

Usage
-----

In any view:

    <% store 'fragment_name', :observe => [:users, :coments] do %>
      cached fragment which does something intensive
    <% end %>

This fragment will be cached until a save or destroy occur in the User and Comment models.

Installation
------------

You can install it as a Rails plugin or as a gem:

    $ gem sources -a http://gems.github.com (you only have to do this once)
    $ sudo gem install citrusbyte-store_observer

License
-------

Copyright (c) 2008 Michel Martens and Ben Alavi for Citrusbyte

Permission is hereby granted, free of charge, to any person
obtaining a copy of this software and associated documentation
files (the "Software"), to deal in the Software without
restriction, including without limitation the rights to use,
copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the
Software is furnished to do so, subject to the following
conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
OTHER DEALINGS IN THE SOFTWARE.
