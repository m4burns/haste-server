## Basic Usage

Type what you want me to see, click "Save", and then copy the URL.  Send that
URL to someone and they'll see what you see.

To make a new entry, click "New" (or type 'control + n')

## From the Console

Setup (put this in a .profile)

haste() { a=$(cat); curl -X POST -s -d "$a" http://paste.dev.d2l/documents | awk -F '"' '{print "http://paste.dev.d2l/"$4}'; }

Then:

cat something | haste

## Author

* [haste-server](https://github.com/seejohnrun/haste-server)

Code by John Crepezzi <john.crepezzi@gmail.com>
Key Design by Brian Dawson <bridawson@gmail.com>
