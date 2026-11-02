Dictionary corpus input
=======================

The pack build reads every *.txt file in this folder as the dictionary
corpus and derives word frequencies from it.

The release build used a ~12 MB sample of Welsh Wikipedia (cywiki) text.
That sample is NOT tracked in this repository (it exceeds the file-push
limits of the route used to publish this repo, and it is a derived extract
of Wikipedia rather than original code).

To reproduce the release dictionary, download the Welsh Wikipedia dump
from Wikimedia (https://dumps.wikimedia.org/cywiki/), extract plain text,
and place it here as a .txt file before building. Any large Welsh text
corpus works — the dictionary's frequencies follow whatever corpus you
feed it. Wikipedia text is CC BY-SA.

The spoken-layer wordlist (../prebuilt/welsh_spoken.xml) is tracked in the
repo and merges over whatever corpus you use.
