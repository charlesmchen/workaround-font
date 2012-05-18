workaround-font
===============

History
-------

* May 5th, 2012 - started work.

Optical Correction, etc.
------------------------

* Horizontal strokes are slightly thinner than vertical strokes.  
* Diagonal strokes widths fall somewhere in between, varying with the angle of the stroke.
* The rounded terminals and edges are not circular; they are slightly oval in proportion with the horizontal / vertical stroke thickness.
* Rounded terminals descend slightly below the baseline and above the ascender height.
* No tapering on strokes; all straight strokes are mono-width, ie. their sides are parallel.
  * No longer true.  I've tapered the joints on 3, 8, etc. and the counters on O, 0, C, D, etc.

TODOs
-----

* We need to audit all glyph widths.  
* We need to audit all kerning.  
* Is x-height right?
* Is the Cap-A crossbar height right?
* Is the Cap-A crown radius right?
* Is the Cap-A glyph width right?
* When we use connectPathSegments to finalize complicated paths, do we end up with irrational
   segments?  Should we modify connectPathSegments() to modify in-place adjoining segments with 
   close (re: a specific tolerance) endpoints?
* The Cap-A is bad.
* The Cap-A is tricky.
* The Cap-B is tricky.
* The Cap-G is very tricky.
* The Cap-J is tricky.
* The Cap-K is tricky.
* The Cap-M is outright bad.  inverting the w isn't good enough.
* The Cap-R is tricky.
* Should the foot of the Cap-R leg flush to the baseline or rotated square to the leg?
* The 2 is tricky.
* The 7 is outright bad. 
* The 8 is tricky. 
* Fix the crossbars in the cap and lowercase z's.
* The descenders are completely fubar'd.
	* FIXED
* The bdpq is bad.
* The e is bad and adapts poorly to semiround/bold.
	* BETTER
* The g tail needs to be stretched.
	* BETTER
* the g italics are fubar-ed.
	* FIXED
* The x-height is probably too low
	* BETTER
* the s has severe problems, especially in bold.  raising the x-height will probably help.
* the t foot is way too curved.
	* NEEDS WORK
* the x tips should probably not be tipped.
	* BETTER
* the z diagonal should be thinned.
 
* We need to compare various cross-bars and make sure they align.
  * A, S, F, G, H, K, E, R, Y, P, B, X, 
  * Numerals too!, ie. 3, 4, 5, 6, 8, 9.
  * etc.

Links
-----

http://www.myfonts.com/search/tag%3Arounded/fonts/?sort=sales
http://www.myfonts.com/search/tag%3Around/fonts/?sort=sales

Interesting idea from: Albert-Jan Pool
http://en.wikipedia.org/wiki/Clothoid
