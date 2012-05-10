workaround-font
===============

Optical Correction

* Horizontal strokes are slightly thinner than vertical strokes.  
* Diagonal strokes widths fall somewhere in between, varying with the angle of the stroke.
* The rounded terminals and edges are not circular; they are slightly oval in proportion with the horizontal / vertical stroke thickness.
* Rounded terminals descend slightly below the baseline and above the ascender height.
* No tapering on strokes; all straight strokes are mono-width, ie. their sides are parallel.
  * No longer true.  I've tapered the joints on 3, 8, etc. and the counters on O, 0, C, D, etc.

TODOs:
* We need to audit all glyph widths.  
* We need to audit all kerning.  
* Is x-height right?
* Is the Cap-A crossbar height right?
* Is the Cap-A crown radius right?
* Is the Cap-A glyph width right?
* When we use connectPathSegments to finalize complicated paths, do we end up with irrational
   segments?  Should we modify connectPathSegments() to modify in-place adjoining segments with 
   close (re: a specific tolerance) endpoints?
* The Cap-G is very tricky.
* The Cap-J is tricky.
* The Cap-R is tricky.
* The Cap-A is tricky.
* The Cap-A is outright bad.
* The Cap-B is tricky.
* The Cap-K is tricky.
* The Cap-M is outright bad.  inverting the w isn't good enough.
* Should the foot of the Cap-R leg flush to the baseline or rotated square to the leg?

* We need to compare various cross-bars and make sure they align.
  * A, S, F, G, H, K, E, R, Y, P, B, X, 
  * Numerals too!, ie. 3, 4, 5, 6, 8, 9.
  * etc.
  
http://www.myfonts.com/fonts/bomparte/glow-gothic/overlay/glyphs.html
http://www.myfonts.com/fonts/g-type/chevin-pro/bold/glyphs.html
http://www.myfonts.com/fonts/typodermic/scheme/regular/glyphs.html
http://www.myfonts.com/fonts/typodermic/report/semibold/glyphs.html

http://www.fontshop.com/fonts/downloads/fontfont/ff_speak_web/
http://www.fontshop.com/fonts/downloads/fontfont/ff_din_round_web/

http://www.myfonts.com/search/tag%3Arounded/fonts/?sort=sales
http://www.myfonts.com/search/tag%3Around/fonts/?sort=sales

http://www.behance.net/gallery/FF-DIN-Round/647150
Interesting idea from: Albert-Jan Pool
http://en.wikipedia.org/wiki/Clothoid
