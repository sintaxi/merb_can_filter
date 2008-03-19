= merb_can_filter

http://rubyforge.org/projects/sintaxi/

== DESCRIPTION:

Filters from your choice of Markdown, Textile or Plain HTML into
HTML and gives appropriate markup for syntax highlighting on code.

== FEATURES/PROBLEMS:

* Formats Textile or Markdown
* Applies markup to code for syntax highlighting.
* requires a filter(string) column

== SYNOPSIS:

In any model specify what columns to filter and how it should
be filtered using a 'filter' column with a value of Markdown, 
Textile or Plain HTML.

  merb_can_filter :body, :excerpt

In this case the filtered(html) data will be saved to body_html 
and excerpt_html (be sure those columns exist in your database.

All instances of <code></code> will have markup for syntax 
highlighting. Specify your markup language eg. <code:ruby></code>
or <code:javascript></code>

== REQUIREMENTS:

* RedCloth
* BlueCloth
* CodeRay

== INSTALL:

* sudo gem install merb_can_filter

== LICENSE:

(The MIT License)

Copyright (c) Brock Whitten 2008

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
