SCSSFRCSS
==========

Welcome to SCSSFRCSS.

SCSSFRCSS is an open source, basic Sass file structure influenced by SMACSS.

##CHANGING FILE EXTENSIONS VIA THE COMMAND LINE

If you are interested in working with `.scss` files instead of the standard `.sass` files to faciliate more easily structurable logic, simply `cd` into the sassafrass directory and run

    find -name '*.sass' -exec rename -n 's/sass$/scss/' {} \;

in the command line.  If working in a rails environment, enter

    find -name '*.sass' -exec rename -n 's/sass$/css.scss/' {} \;

instead. The `-n` flag will run through the directory and list the proposed changes.  If the listing is correct, simply rerun the command, replacing the `-n` with a `-v`.

The `sass$` insures that a file that contains "sass" will not be changed; it only looks at the end of the file, i.e. `sass.sass` will become `sass.scss`.

***

Many thanks to the teachings of Dale Sande, AKA [anotheruiguy](https://speakerdeck.com/anotheruiguy).
Props to jdubjdub for the name.

Copyright (c) 2014 Brian Studwell

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.


