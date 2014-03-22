# HoTT Type

Homotopic Type Theory for ordinary mortals.

## Status

Currently this document consists of the introduction and first chapter
of [the HoTT Book](http://homotopytypetheory.org/book/) ([github
repo](https://github.com/HoTT/book)), plus a section of notes.

## Point

The HoTT Book is excellent, but is aimed at a fairly sophisticated
audience.  Most of the mathematics is over my head.  The more basic
stuff about types, judgments, etc. I think I understand (I have read
Martin-Lof's papers, and lots of other related stuff), but I find some
of the explanations in the intro and chapter 1 a little murky.

I'd like to eventually turn this into a bona fide guide to HoTT for a
non-specialist audience, with particular focus on your working stiff
programmer.  Recently I've come across some online discussions about
dependently typed languages, among pretty sophisticated programmers
and language designers, that lead me to think that the real
significance of type theory is not particularly well-understood even
among the technical cognoscenti.  There seems to be a persistent
inclination to think of a type as a kind of fancy or mysterious set,
when in fact it is something entirely different (at least as far as I
can tell).

But for the moment, this is where I dump my notes as I work my way
through the bits of the HoTT Book that I am capable of understanding.
With liberal quotations from Martin-Lof and other major figures
(Frege, Wittgenstein, Dummett, and especially Brandom.)

## Plan

### Content

* add language-specific examples to section Type Theory (HoTT ch. 1)

* explicate philosophical foundations of type theory.  Martin-Lof was
specific: his original motivation was "solely philosophical".  To some
extent the center of HoTT is a philosophical topic, one of the most
important in 20th century philosophy: the nature of propositions,
judgments, assertions, etc.

* HoTT Book chapter 1 contrasts the bilevel nature of set theory+logic
  on the one hand and type theory on the other.  This is excellent,
  but needs more elaboration for those of us who don't speak
  first-order logic as a second language.  Some specific examples
  illustrating the difference would be very helpful.

* Contrast of sets and types: this strikes me as not only fundamental
  but easy to under-appreciate.  It seems to me that ultimately set
  theory and type theory represent radically different ways of
  thinking.  The HoTT Book, chapter 1, does a fairly good job of
  drawing the distinction, but at a relatively superficial level; it
  could use more detail, plus some concrete examples, in my opinion.

* _a : A_ as analogue of proper noun plus description, e.g. King
  George, President Washington, General Custer, Seargeant York,
  Chicken George, Slick Willy, Ivan the Terrible, Joan of Arc, Crazy
  Eddy, maybe Joe Sixpack, Joe the Plumber, Law-school LIz, Commie Bryan, etc.

* Martin-Lof on judgment, proposition, assertion, etc.

* Geach on assertion: the Frege Point.  "A thought may have just the
same content whether you assent to its truth or not; a proposition may
occur in discourse now asserted, now unasserted, and yet be
recognizably the same proposition. . . . I shall call this point about
assertion the Frege point. . ." Geach, "Assertion" (Some call this the
Geach-Frege Point)

* Brandom on assertion as commitment + entitlement

### Organization

???

### Formatting and Style

* Liberate the text from the HoTT Book latex: get rid of the index
  stuff, etc. and in general simplify.  Use [tufte-latex](https://code.google.com/p/tufte-latex/), with side and
  margin notes, etc.

* Convert to XML and write some XSL styleshoots to produce a dazzling
  adaptive animated etc. HTML5 web site.  For example I'd like to
  emulate tufte's style; something approaching that (at least, with
  marginnotes) using HTML5 tags is at
  (http://bost.ocks.org/mike/join/)


* etc.