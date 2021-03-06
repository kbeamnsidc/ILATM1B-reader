# Matlab ILATM1B Reader Release Notes

## Release v0.4 (2018-02-07)

* Created MATLAB package `ilatm1b`.

* Renamed functions `read` and `test_read`.

* Added a LICENSE (MIT License).

## 2014-04-17

* Changed version to '0.3' in readILATM1B.m.

* Changed n4ftl01u.ecs.nasa.gov to n5eil01u.ecs.nsidc.org in:
  
  * matlab-ILATM1B-reader-readme.txt
  * readILATM1B.m
  * test_readILATM1B.m

* Added RELEASE_NOTES.txt to matlab-ILATM1B-reader-readme.txt

Added matlab_ILATM1B-reader_0.3.tar

## 2013-05-14

* Fixed bug in readILATM1B.m first reported by Ben Panzer at CReSIS
such that the program would return different sized arrays on
subsequent calls using the same input file. Ben suggested removing the
& from the unix() call to qi2txt so that readILATM1B.m waits for
qi2txt to finish processing before readILATM1B.m reads the output file
produced by qi2txt. Implemented Ben's suggestion.

* Added returned header value.

* Added use of Matlab tempname function in place of hard-coded temporary
file names.

* Added creation and display of version string.

* Removed example_output_readILATM1B.txt and created
test_readILATM1B.m and associated expected_output.txt which is a link
to ../C/example_output.txt.

* Added make_tarball.pl.

* Added matlab_ILATM1B_reader_0.2.tar.

* Added RELEASE_NOTES.txt
