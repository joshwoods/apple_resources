

- QuickTime File Format
-  Reference movie descriptor atom ('rmda') 

Atom

# Reference movie descriptor atom ('rmda')

An atom that contains other atoms that describe where to find a particular movie, the system requirements to play that movie, and a quality rating.

## Overview

The reference movie descriptor atom contains other atoms that describe where a particular movie can be found, and optionally what the system requirements are to play that movie, as well as an optional quality rating for that movie.

A reference movie descriptor atom’s parent is always a movie reference atom (`'rmra'`). Multiple reference movie descriptor atoms are allowed in a given movie reference atom, and more than one is usually present.

## Topics

### Data fields

Size

The number of bytes in this reference movie descriptor atom.

Type

The type of this atom.

Data reference atom

Each reference movie atom must contain exactly one data reference atom.

Data rate atom

A reference movie atom may contain an optional data rate atom.

CPU speed atom

A reference movie atom may contain an optional CPU speed atom.

Version check atom

A reference movie atom may contain an optional version check atom.

Component detect atom

A reference movie atom may contain an optional component detect atom.

Quality atom

A reference movie atom may contain an optional quality atom.

## See Also

### Describing reference movies

Reference movie atom ('rmra')

A reference movie atom contains references to one or more movies.

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

