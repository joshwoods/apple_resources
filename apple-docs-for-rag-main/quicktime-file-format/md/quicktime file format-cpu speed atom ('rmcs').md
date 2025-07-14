

- QuickTime File Format
-  CPU speed atom ('rmcs') 

Atom

# CPU speed atom ('rmcs')

A CPU speed atom specifies the minimum computing power needed to display a movie.

## Overview

A CPU speed atom specifies the minimum computing power needed to display a movie. QuickTime performs an internal test to determine the speed of the user’s computer.

This is not a simple measurement of clock speed — it is a measurement of performance for QuickTime-related operations. Speed is expressed as a relative value between `100` and `2^31`, in multiples of `100`.

Applications play the movie with the highest specified CPU speed that is less than or equal to the user’s speed. If the user’s speed is lower than any movie’s CPU speed, applications play the movie with the lowest CPU speed requirement. The movie with the highest CPU speed is assumed to be the highest quality.

Only one CPU speed atom is allowed in a given reference movie descriptor atom.

## Topics

### Data fields

Size

The number of bytes in this CPU speed atom.

Type

The type of this atom.

Flags

A 32-bit integer that is always 0.

CPU speed

A relative ranking of required computer speed, expressed as a 32-bit integer divisible by 100, with larger numbers indicating higher speed.

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

Version check atom ('rmvc')

A version check atom specifies a software package, such as QuickTime or QuickTime VR, and the version of that package needed to display a movie.

Component detect atom ('rmcd')

A component detect atom specifies a QuickTime component, such as a particular video decompressor, required to play the movie.

Movie importer component flags

Flags that adjust the behavior of the movie import component.

Quality atom ('rmqu')

A quality atom describes the relative quality of a movie.

