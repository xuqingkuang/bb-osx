What is this fork
=================
This is AA-Project's classic Demo "BB" with some fixes applied to allow it to build on modern Macs and run at absurdly high resolutions (2880x1800 text mode!).

How to build and run:

First clone/downlaod this repository
```
cd bb-osx
brew install libmikmod aalib
```

For compling on Apple Silicon architecture. (compling issue still exist)
```
./configure
make
```

For compiling on x86-64 architecture.
```
./configure --with-aalib-exec-prefix=/opt/homebrew --with-libmikmod-exec-prefix=/opt/homebrew
make
```

Then execute `./bb` to run.

Note: `./configure` sometimes needs the path to `libmikmod` passed manually. This can be done with `--with-libmikmod-prefix=[prefix]`.
Note: Audio may not play, this looks like a bug.

What does this software do then ?
=================================

	BB is an high quality audio-visual demonstration for your text
terminal. It is portable demo, so you can run it on plenty of operating 
systems and DOS. 

Supports: dos (VGA + MDA), stdio, curses, slang, X11, gpm, linux-console
Sound:  OSS, Sun audio, SGI, DEC Aplha, AIX, HP-UX, DOS (GUS CLASSIC, GUS
        CLASSIC, GUS MAX, GUS ACE, GUS PNP, SB, ESS, PC-buzzer 

How this all started
====================

   Once upon a time we've (my friend Kamil and I) bought two old
Herculeses as secondary monitors. We didn't know for that time that our
Diamond Stealths 64 cards would become obsolete soon. The next day we
downloaded the logo of Linux Texas Users Group - nice silly penguin
looking like a cowboy! It was so exciting logo ... we decided that we
couldn't live without it and we wanted to see it at boot time as a logo
on our secondary monitors. There was a small problem - Hercules doesn't
support color graphics. So we decided to convert the penguin image to
ascii art using netpbm tools.

   The output was very ugly because the converting algorithm was
absolutly stupid.  During the night I designed a new convertor that
used a font bitmap to creat an aproximation table. The output wasn't
very good since the algorithm wasn't tuned so well. Many months this
small piece of code was waiting on my disc for the day "D". Meanwhile I
started a new project XaoS (a fractal zoomer) with my friend Thomas.
And then I got an idea: Ascii Art Mandelbrots!  I was really impressed
by the result! XaoS was faster, portable and looking much better than
ever before. I found a new way to go ...


AA-Project
==========

                               dT8  8Tb
                              dT 8  8 Tb
                             dT  8  8  Tb
                          <PROJECT><PROJECT>
                           dT    8  8    Tb
                          dT     8  8     Tb
   
Three goals of AA-Project:

  1. Port all important software (like Doom, Second Reality, X windows
     etc..) on AA-lib.

  2. Port AA-lib on all available platforms (mainly ZX-Spectrum and
     Sharp).

  3. Force IBM to start manufacturing MDA cards again.

   AA-project was started by Jan Hubicka. In that times just a few
people knew about it. Then a new demo named BB has been relased to show
the power of AA-lib technology. Now the project is freely available and
anyone can help.

Where to find BB
================

   All programs covered under AA-project can be obtained at
`http://aa-project.sourceforge.net'.

Support us:
===========

   We decided to distribute all of our aa-related programs freely (see
COPYING for details). If you want to help us more (so we could develop 
more such software) send a small amount (or big one ;-) to AA/BB team.
In that case, write us for further instructions...

kupsaf@feld.cvut.cz (Filip Kupsa)
hubicka@freesoft.cz (Jan Hubicka)
titania@horac.ta.jcu.cz (Mojmir Svoboda)
toman@atrax.karlin.mff.cuni.cz (Kamil Toman)
