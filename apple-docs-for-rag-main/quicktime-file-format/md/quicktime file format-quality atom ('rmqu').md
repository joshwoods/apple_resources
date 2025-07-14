

- QuickTime File Format
-  Quality atom ('rmqu') 

Atom

# Quality atom ('rmqu')

A quality atom describes the relative quality of a movie.

## Overview

This acts as a tiebreaker if more than one movie meets the specified requirements, and it is not otherwise obvious which movie should be played.

This would be the case if two qualified movies have the same data rate and CPU speed requirements, for example, or if one movie requires a higher data rate and another requires a higher CPU speed, but both can be played on the current system. In these cases, applications play the movie with the highest quality, as specified in the quality atom.

Only one quality atom is allowed in a given reference movie descriptor atom.

## Topics

### Data fields

Size

The number of bytes in this quality atom.

Type

The type of this atom.

Quality

The relative quality of the movie, expressed as a 32-bit integer.

## See Also

### Describing reference movies

Reference movie atom ('rmra')

A reference movie atom contains references to one or more movies.

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

