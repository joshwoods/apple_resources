

- QuickTime File Format
-  Reference movie atom ('rmra') 

Atom

# Reference movie atom ('rmra')

A reference movie atom contains references to one or more movies.

## Overview

It can optionally contain a list of system requirements in order for each movie to play, and a quality rating for each movie. It is typically used to specify a list of alternate movies to be played under different conditions.

A reference movie atom’s parent is always a movie atom (`'moov'`). Only one reference movie atom is allowed in a given movie atom.

## Topics

### Data fields

Size

The number of bytes in this reference movie atom.

Type

The type of this atom.

Reference movie descriptor atom

A reference movie atom must contain at least one reference movie descriptor atom, and typically contains more than one.

## See Also

### Describing reference movies

Reference movie descriptor atom ('rmda')

An atom that contains other atoms that describe where to find a particular movie, the system requirements to play that movie, and a quality rating.

Reference movie data reference atom ('rdrf')

An atom that contains the information necessary to locate a movie, stream or file.

Data rate atom ('rmdr')

A data rate atom specifies the minimum data rate required to play a movie.

CPU speed atom ('rmcs')

A CPU speed atom specifies the minimum computing power needed to display a movie.

Version check atom ('rmvc')

A version check atom specifies a software package, such as QuickTime or QuickTime VR, and the version of that package needed to display a movie.

Component detect atom ('rmcd')

A component detect atom specifies a QuickTime component, such as a particular video decompressor, required to play the movie.

Movie importer component flags

Flags that adjust the behavior of the movie import component.

Quality atom ('rmqu')

A quality atom describes the relative quality of a movie.

