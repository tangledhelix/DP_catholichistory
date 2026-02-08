## The Catholic Church and History - 623ad113028e7 ##

This is a [Distributed Proofreaders](http://www.pgdp.net/) post-processing project.

“The Catholic Church and History” by Belloc, Hilaire

* [DP project page](http://www.pgdp.net/c/project.php?id=projectID623ad113028e7)
* [Forum thread](https://www.pgdp.net/phpBB3/viewtopic.php?t=76504)
* [Good words](good_words.txt)
* [Bad words](bad_words.txt)
* [Project Gutenberg listing]() (not posted yet)

Page references (e.g. `001`) refer to the scan numbers, not the original book's page numbers.

### Things to revisit ###

* [x] review book structure (see notes below) for any h3 needed
* [x] 027: complex table
* [x] 070: footnote using Greek transliteration; change to utf8
* [x] 096: question about `nor here` vs `nor there` - review in TIA scans

### Project manager notes ###

<div style="text-align:center"><h3>ABOUT THE BOOK</h3></div>

<h4>Author</h4>

<p><a href="https://en.wikipedia.org/wiki/Hilaire_Belloc">Hilaire Belloc</a> (1870-1953).</p>

<h4>Publication date</h4>

<p>1926.</p>

<h4>Source.</h4>

<p> The page images were  <a href="https://archive.org/details/catholicchurchhi0000bell"> taken from here</a>.</p>

<hr />

<div style="text-align:center"><h3>PROOFING</h3></div>

<p><b>Difficulty level:</b> Easy.</p>

<p>Wordcheck is <b>mandatory</b> in the P2 and P3 rounds; I respectfully request that P1 proofers use it as well.</p>

<p>The Maltese cross (✠) has been added as a custom character for this project.</p>

<hr />

<div style="text-align:center"><h3>FORMATTING</h3></div>

<p><b>Difficulty level:</b> Easy.</p>

<hr />

<p>There are no special instructions for this book. Please
follow the normal <a href="https://www.pgdp.net/wiki/DP_Official_Documentation:Proofreading/Proofreading_Guidelines">Proofing</a> and <a href="https://www.pgdp.net/wiki/DP_Official_Documentation:Formatting/Formatting_Guidelines">Formatting Guidelines</a>.</p>

<p>Questions may be posted in the Project Forum (link above).</p>

<hr />

<div style="text-align:center"><h3>POST PROCESSING</h3></div>

<p><b>Difficulty level:</b> Easy.</p>

### Forum notes ###

### General notes ###

Book structure: Seems to be 4 major divisions that I'll treat as chapters. Whether to create h3 sections is something to think about for later.

```
005 Preface
007 Editor's Preface
013 Book begins with I

013 I
    1. 2. 3.
016 II
    (1) (2) (3)
021 III
    (I)
        (a) (b) (c)
    (II)
        (a) (b)
026 IV
    (I)
        (a) (b) (c)
    (II)
        (a) (b)
```

[Posted](https://www.pgdp.net/phpBB3/viewtopic.php?p=1387095#p1387095) in forum about Greek word in footnote on page 70. Confirmed with the experts.

### Illustrations ###

None.

### Proofer's notes ###

### Joined hyphenated words ###

### Spellcheck ###

### Transcriber's notes ###

TXT: italics, smallcaps

p. 37: changed “phenomenom” to “phenomenon” (That such a phenomenon)

p. 48: deleted duplicate word “the” (condemned by authority of the Catholic Church)

p. 71: changed “eraliest” to “earliest” (the earliest origins of the Church)

p. 83: changed “men” to “man” (first the teacher is a revered man)

p. 96: changed “cay” to “may” (what we may say with regard to)

p. 96: changed “here” to “there” (neither here nor there)

### HTML file review ###
The iPhone/iPad simulators can't use `file://` URLs. Start a local web server with `python3 -m http.server` in the project directory and going to `localhost:8000` in Safari on the device. 

* [x] Safari
* [x] Firefox
* [x] Chrome
* [x] iPhone simulator
* [x] iPad simulator

### Ebook review ###

* Surprisingly, the wide table is scrollable in ADE
  * Although the brace height sizing isn't quite as good as in browsers.
  * [ ] should I leave the "scroll" notice in the EPUB??
* The table renders nicely (but small) in Apple Books Mac.
  * Clicking on it brings it to full size and it's quite readable.
  * No opportunity given to scroll, on Mac at least.
* Kindle (previewer, even as tablet) does a very bad job with the table.
  * Re-try without overflow-x? Seems about the same.
  * Kindle zoom, usually a godsend for tables, does badly here
  * It doesn't seem to honor the height sizing of the braces...
  * Nor the width for the table cells.
  * "set up and electrotyped" paragraph not centered
* Calibre does fine with the book overall
  * But the table is clipped off screen. No ability to scroll.
  * Without the overflow-x:auto it's worse; it overlaps text on the next page turn
* Kobo: the iron cross symbol for the imprimatur is not rendered
  * "set up and electrotyped" paragraph not centered
  * Kobo somehow does even worse on the table. It only renders part of it, but also shows a scrollbar... but you can't *use* the scrollbar!
  * Renders the Greek word, although it renders as if it has letter-spacing active.
* Apple Books on iPhone does render "electrotyped" paragraph as centered
  * It does OK with the table - you can click it to get a full view that is zoomable with pinch. However, it doesn't size the braces right, they are rendered presumably at their native resolution.
* Kindle on iPhone shows the "electrotyped" paragraph as left margin
  * Renders the table accurately, and you can click in and zoom, but the rendering leaves a lot to be desired, including that the braces are not rendered at the correct sizes.
* Google Play Books may take the cake. It seems when you reach the table it just starts showing a "loading" spinner. You can page backward, to get back into the book, but then it just won't go past there?! Wow.
  * [ ] How to deal with this? Is it due to overflow-x or something? Maybe put the overflow-x in a class that can be dropped for ebookmaker?
  * Seems that's not it; I took the overflow-x bit out and it still fails. Wow!

### Smooth Reading ###

smoothread_01.txt:

```
In the Protestant thesis of the mid-Victorian
day the corruption began about the end of the second century. St. Paul
was accepted, but already there was trouble beginning, as revealed in
the authentic epistles of St. Ignatius; and manifestly things were
becoming Catholic (and therefore corrupt) by the time of the African
Martyre[**Martyrs?], and were hopeless by the time of the Thirty Tyrants.
```

This seems to be an archaic, but valid, spelling, and the kind of thing Belloc was known to do. Leaving as-is.
