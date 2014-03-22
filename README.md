# HoTT Type

Homotopic Type Theory for ordinary mortals.

## Status

Currently this document consists of the introduction and first chapter
of [the HoTT Book](http://homotopytypetheory.org/book/) ([github
repo](https://github.com/HoTT/book)), plus a section of notes.  The
HoTT Book is published under the Creative Commons
Attribution-ShareAlike 3.0 Unported License, so I'm assuming the
authors actually want people not just to read it but to do stuff with
it, like create derived works.  Or, in this case, create mashups based
on it.

## Point

The HoTT Book is excellent, but is aimed at a fairly sophisticated
audience.  Most of the mathematics is over my head.  Not that I'm
uninterested in the math; I just don't have the time to study it.  So
my main interest in the HoTT Book is as a route to programming with
dependent types.  The more basic stuff about types, judgments, etc. I
think I understand (I have read Martin-Lof's papers, and lots of other
related stuff), but I find some of the explanations in the intro and
chapter 1 a little murky.

There are lots of papers, tutorials, etc. about dependent types and
intuitionistic type theory freely available on the web.  Why the HoTT
Book?  Well, for one thing it aims at presenting a foundation of
mathematics; so there is a clear contrast with set theory.  For
another, it's pretty readable, at least the intro and chapter 1 are,
even for non-mathematicians.

I'd like to eventually turn this into a bona fide guide to HoTT for a
non-specialist audience, with particular focus on your working stiff
programmer.  Retaining most of the text taken from the HoTT Book but
adding some commentary, notes, guides, etc.  Recently I've come across
some online discussions about dependently typed languages, among
pretty sophisticated programmers and language designers, that lead me
to think that the real significance of type theory is not particularly
well-understood even among the technical cognoscenti.  There seems to
be a persistent inclination to think of a type as a kind of fancy or
mysterious set, when in fact it is something entirely different (at
least as far as I can tell).

But for the moment, this is where I dump my notes as I work my way
through the bits of the HoTT Book that I am capable of understanding.
With liberal quotations from Martin-Lof and other major figures
(Frege, Wittgenstein, Dummett, and especially Brandom.)

See [Topoi: The Categorial Analysis of
Logic](http://ebooks.library.cornell.edu/cgi/t/text/text-idx?c=math;idno=gold010)
for an excellent example of technical exposition of arcana.  Goldblatt
explains the basics of category theory in simple and intuitive terms,
often by comparing the CT way of seeing with the set theoretic way.
The HoTT Book is already pretty good at this but I'd like a (reduced)
version that targets the reasonably well-informed practicing
programmer rather than the mathematician.  For example, I'd like to
see an explicit discussion of the contrast between the classical way
of understanding the quantifiers versus the type theoretic way.
(First step: explain what problem was solved by the invention of
quantifiers, and why were they a good solution; then, what problem
does type-theoretic quantification solve.  Etc.  In this case, the
classic quantifiers do not pick out determinate individuals
(witnesses).  This might be trivial for trained mathematicians and
logicians, but it's not for the rest of us.  Compare the subtleties of
material implication, which seems so simple on the surface.)

## Plan

### Content

* add language-specific examples to HoTT ch. 1.

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
  drawing the distinction, but is very concise; it could use more
  detail, plus some concrete examples, in my opinion.

* Add contrasting set-theoretic examples wherever type-theoretic
  concepts are explained.  It makes it a lot easier to see what's
  going on if you can relate the unfamiliar stuf to what you already
  know.

* The relation between the "things" and inference.  HoTTB chapter 1
  offers a very concise account of this, which I understand to mean
  that inference in set theory is "external" to its objects (sets),
  while in type theory inference is intrinsic to its objects (types,
  whose constructors etc. are "internal" to the system; or something
  like that).  This could use a more detailed elaboration.

* What's the deal with induction and quantification?  The relation
  between classic predicate logic and dependent type theory could be
  made more clear.  Quantification, for example, is non-procedural in
  classic logic - you quantify over a domain conceptually, but you
  don't say *how* that is done - and type theory provides procedural
  analogues for the quantifiers.  For non-specialists learning
  dependent type theory stuff like this really helps develop
  intuition.  IOW one way of looking at the task is: given the
  essentially non-procedural concepts of set theory and classic logic
  that we all know and love, come up with a way of capturing the same
  basic ideas as procedures.

* _a : A_ as analogue of proper noun plus description, e.g. King
  George, President Washington, General Custer, Seargeant York,
  Chicken George, Slick Willy, Ivan the Terrible, Joan of Arc, Crazy
  Eddy, maybe Joe Sixpack, Joe the Plumber, Law-school LIz, Commie Bryan, etc.

* Gentzen on natural deduction.  Prawitz.

* Martin-Lof on judgment, proposition, assertion, etc.

* Geach on assertion: the Frege Point.  "A thought may have just the
same content whether you assent to its truth or not; a proposition may
occur in discourse now asserted, now unasserted, and yet be
recognizably the same proposition. . . . I shall call this point about
assertion the Frege point. . ." Geach, "Assertion" (Some call this the
Geach-Frege Point)

 * my understanding of "judgment" as explained in Chapter 1 section 1
   is that it amounts to an intrinsically asserted proposition, one
   that always carries assertional force.  That's why *a : A* cannot
   be embedded as the antecendent in a conditional; conditional
   antecedents are always unasserted propositions, and *a : A* is
   intrinsically an assertion (judgment).

* Brandom on assertion as socially articulated commitment +
  entitlement, and how this can be used to explicate the concept of
  judgment in HoTT.

* HoTTB chapter 1 presents a mathematical view of deductive systems,
  likening them to formal games where judgments are "positions", or to
  algebras where judgments are elements and deductive rules are
  operations, etc.  That's fine as far as it goes, but in the end I
  think it inadequate and even somewhat misleading.  Assertion,
  judgment, etc. are things that only people can do.  Treating them as
  mathematical abstractions, e.g. a move in a game, algebraic
  operation, etc., inevitably "loses the phenomenon".  In other words,
  it is not correct to say things like "P is a judgment" or assertion,
  since judgments/assertions always involve both a judger/asserter and
  what gets judged/asserted.  So we need an account of what it means
  to say "P is an assertion" when refering to a P written in a
  mathematical text.  It must mean something like "convention says
  readers should _treat_ the written expression as if it had been
  asserted by somebody" - in other words, its a normative affair
  involving assumptions or stipulations.

* Something about proof assistants.

  * more on the connection between the math side of things and the (automated) proof side of things

  * maybe some kind of basic intro to using proof assistants.  it's not
   easy to find good intros to this; for example, one often comes
   across references to "tactics", but I've never come across a
   concise and clear explanation of what they are

  * I'm thinking specifically about Agda, ATS, and Idris - tools you
   can use to actually write programs

### Organization

???

### Formatting and Style

* Liberate the text from the HoTT Book latex: get rid of the index
  stuff, etc. and in general simplify.  Use [tufte-latex](https://code.google.com/p/tufte-latex/), with side and
  margin notes, etc.

* Convert to XML and write some XSL stylesheets to produce a dazzling
  adaptive animated etc. HTML5 web site.  For example I'd like to
  emulate tufte's style; something approaching that (at least, with
  marginnotes) using HTML5 tags is at
  (http://bost.ocks.org/mike/join/)


* etc.