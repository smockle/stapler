[![Build Status](https://travis-ci.org/smockle/stapler.svg?branch=master)](https://travis-ci.org/smockle/stapler)

Stapler
=======

Stapler manipulates PDFs using Prawn.

Usage
=====

    # Copy the specified page to a new PDF.
    stapler get input.pdf [output.pdf] 4
    
    # Copy the specified pages to a new PDF.
    stapler get input.pdf [output.pdf] 4..42

    # Insert a PDF before the specified page.
    stapler insert input.pdf insert.pdf [output.pdf] 4

    # Merge specified PDFs into a single PDF. 
    stapler join input_1.pdf input_2.pdf output.pdf

    # Merge all PDFs into a single PDF.
    stapler join *.pdf output.pdf

    # Remove the specified page.
    stapler remove input.pdf [output.pdf] 4
    
    # Remove the specified pages.
    stapler remove input.pdf [output.pdf] 4..42

    # Split the pages of input.pdf into multiple PDFs.
    stapler split input.pdf
    
License
=======

Stapler is released under the MIT License.

Stapler requires the Thor and Prawn gems. Thor is licensed under the MIT License. Prawn is dual-licensed under the Ruby License and the GPL. The [Ruby License](http://www.ruby-lang.org/en/about/license.txt) permits redistribution and modification under the 2-clause BSD License, which is compatible with the MIT License.