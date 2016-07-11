# ham4corpus
The #ham4corpus repo currently contains files with various types of information about the Original Broadway Cast recording of Hamilton: An American Musical (i.e. all words currently in the show, minus the one scene not on the OBC recording).

*Suggested uses:* Twitter bots, text visualization. 

All lyrics are by Lin-Manuel Miranda. 

# The files
## Lyrics, including character names before their parts
**Title:** All_Hamilton_Lyrics_Speakers

**What:** One file containing all lyrics sung in the Original Broadway Cast recording of Hamilton: An American Musical, with the name of the character singing each part appearing on the line above the beginning of their part. No empty lines between anything, just a solid block of Hamilton. Copied and pasted from the lyrics on Genius.com; the placement of simultaneous lyrics is broken up rather than side-by-side.

**Pulled from:** http://genius.com/albums/Lin-manuel-miranda/Hamilton-original-broadway-cast-recording

## Lyrics, not including character names before their parts
**Title:** All_Hamilton_Lyrics_No_Speakers

**What:** One file containing all lyrics sung in the Original Broadway Cast recording of Hamilton: An American Musical. No empty lines between anything, just a solid block of Hamilton.  Copied and pasted from the lyrics on Genius.com; the placement of simultaneous lyrics is broken up rather than side-by-side.

**Pulled from:** http://genius.com/albums/Lin-manuel-miranda/Hamilton-original-broadway-cast-recording

## Original Broadway Cast Actors & Character Names
**Title:** OBC_Cast_Actors_Character.json

**What:** Actors and the named characters played by them in the Original Broadway Cast recording of Hamilton: An American Musical. Actors who played multiple characters are listed multiple times.

**Pulled from:** https://en.wikipedia.org/wiki/Hamilton_(musical)#Principal_roles_and_major_casts

# How

I wish I could say my Python is non-rusty enough that I scraped Genius.com and Wikipedia to get this data, but it isn't and I was on hold on the phone, so I just cut and pasted everything into a text document and grepped:

^\s*?\r to remove blank lines

\[.* to remove the [character names]

If you'd like to learn more about doing cool digital things with text, check out [The Programming Historian](http://programminghistorian.org/lessons/) for novice-friendly, peer-reviewed lessons on data cleaning, distant reading, web scraping, and Python.
