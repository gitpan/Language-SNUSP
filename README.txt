NAME
    Language::SNUSP - A SNUSP Interpreter and Visual Debugger

SYNOPSIS
        > snusp examples/fizzbuzz.snusp
        > snusp --trace examples/fizzbuzz.snusp
        > snusp --debug examples/fizzbuzz.snusp

DESCRIPTION
    SNUSP is a two-dimensional programming language described here:

    http://c2.com/cgi/wiki?SnuspLanguage
    http://rosettacode.org/wiki/Category:SNUSP

    Here is the well known FizzBuzz algorithm, written in SNUSP:

                /               'B' @=@@=@@++++#
               // /             'u' @@@@@=@+++++#
              // // /           'z' @=@@@@+@++++#
             // // // /         'i' @@@@@@=+++++#
            // // // // /       'F' @@@=@@+++++#
           // // // // // /      LF  ++++++++++#
          // // // // // // /   100 @@@=@@@=++++#
        $@/>@/>@/>@/>@/>@/>@/\   0
        /                    /
        !                             /======= Fizz <<<.<.<..>>>#
        /                             |      \
        \?!#->+ @\.>?!#->+ @\.>?!#->+@/.>\   |
        /        !          !         !  /   |
        \?!#->+ @\.>?!#->+@\ .>?!#->+@/.>\   |
        /        !         \!===\!    !  /   |
        \?!#->+ @\.>?!#->+ @\.>?!#->+@/.>\   |
        /        !          !   |     !  /   |
        \?!#->+@\ .>?!#->+ @\.>?!#->+@/.>\   |
        /       \!==========!===\!    !  /   |
        \?!#->+ @\.>?!#->+ @\.>?!#->+@/>>@\.>/
                 !          |   |         |
                 /==========/   \========!\=== Buzz <<<<<<<.>.>..>>>#
                 |
                 \!/=dup==?\>>@\<!/back?\<<<#
                   \<<+>+>-/   |  \>+<- /
                               |
        /======================/
        |
        |       /recurse\    #/?\ zero
        \print=!\@\>?!\@/<@\.!\-/
                  |   \=/  \=itoa=@@@+@+++++#
                  !     /+ !/+ !/+ !/+   \    mod10
                  /<+> -\!?-\!?-\!?-\!?-\!
                  \?!\-?!\-?!\-?!\-?!\-?/\    div10
                     #  +/! +/! +/! +/! +/

    This module installs a SNUSP interpreter so that you can run this code
    yourself. It also installs a visual debugger, to help you follow the
    flow of SNUSP programs.

    Try it. It's very cool!

CREDIT
    This code originated from http://c2.com/cgi/wiki?SnuspLanguage but has
    been fairly heavily refactored to be clear, DRY and conform to modern
    Perl standards.

    I have packaged it on CPAN and GitHub for easy installation and
    continued maintenance.

AUTHOR
    Ingy döt Net <ingy@cpan.org>

COPYRIGHT AND LICENSE
    Copyright (c) 2004. Rick Klement.

    Copyright (c) 2013. Ingy döt Net.

    This program is free software; you can redistribute it and/or modify it
    under the same terms as Perl itself.

    See http://www.perl.com/perl/misc/Artistic.html

