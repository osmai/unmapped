
.osm files for unmapped buildings in england.  compressed hierarchical file layout.

directory/file layout is a tree structure of the form:
ZOOM_18/ab/cd/ef/  where a is the first digit in tiley and b is the first digit in tilex,
                 c is the second digit in tiley and d is the second digit in tilex,
		 etc

file:
ZOOM_18/01/83/41/71.tar
when untarred, will give file(s) e.g.:
ZOOM_18/01/83/41/71/32.tar.gz
which when unzipped and untarred will give file(s) e.g.:
ZOOM_18/01/83/41/71/32/UNMAPPED_ZOOM_18_TILEY_84730_TILEX_131121.osm


Q. WHY THIS FORMAT?
A. people/programs wanting to use this data can download and unzip just the small region that they require,
thus saving on download time and storage.
also, by using gzip and tar, gitlab has less to store.
