

- QuickTime File Format
-  Data rate atom ('rmdr') 

Atom

# Data rate atom ('rmdr')

A data rate atom specifies the minimum data rate required to play a movie.

## Overview

A data rate atom specifies the minimum data rate required to play a movie. This is normally compared to the connection speed setting in the user’s QuickTime Settings control panel. Applications should play the movie with the highest data rate less than or equal to the user’s connection speed. If the connection speed is slower than any movie’s data rate, applications should play the movie with the lowest data rate. The movie with the highest data rate is assumed to have the highest quality.

Only one data rate atom is allowed in a given reference movie descriptor atom.

## Topics

### Data fields

Size

The number of bytes in this data rate atom.

Type

The type of this atom.

Flags

A 32-bit integer.

Data rate

The required data rate in bits per second, expressed as a 32-bit integer.

## See Also

### Describing reference movies

Reference movie atom ('rmra')

A reference movie atom contains references to one or more movies.

Reference movie descriptor atom ('rmda')

An atom that contains other atoms that describe where to find a particular movie, the system requirements to play that movie, and a quality rating.

Reference movie data reference atom ('rdrf')

An atom that contains the information necessary to locate a movie, stream or file.

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

