

- QuickTime File Format
-  Data reference atom 

Atom

# Data reference atom

An atom that contains the information necessary to locate a movie, stream or file.

## Overview

The information to locate a movie, stream, or file is typically in the form of a URL or a file alias. Only one data reference atom is allowed in a given movie reference descriptor atom.

## Topics

### Data fields

Size

The number of bytes in this data reference atom.

Type

The type of this atom.

Flags

A 32-bit integer containing flags.

Data reference type

The data reference type.

Data reference size

The size of the data reference in bytes, expressed as a 32-bit integer.

Data reference

A data reference to a QuickTime movie, or to a stream or file that QuickTime can play.

## See Also

### Describing reference movies

Reference movie atom ('rmra')

A reference movie atom contains references to one or more movies.

Reference movie descriptor atom ('rmda')

An atom that contains other atoms that describe where to find a particular movie, the system requirements to play that movie, and a quality rating.

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

