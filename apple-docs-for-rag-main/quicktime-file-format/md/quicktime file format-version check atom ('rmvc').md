

- QuickTime File Format
-  Version check atom ('rmvc') 

Atom

# Version check atom ('rmvc')

A version check atom specifies a software package, such as QuickTime or QuickTime VR, and the version of that package needed to display a movie.

## Overview

The package is specified using a Macintosh Gestalt type, such a `'qtim'` for QuickTime (QuickTime provides support for these Gestalt tests in the Windows computing environment). You can specify a minimum required version to be returned by the Gestalt check, or you can require that a specific value be returned after performing a binary AND operation on the Gestalt bitfield and a mask. Multiple version check atoms are allowed within a given reference movie descriptor atom. Applications should not attempt to play a movie unless all version checks are successful.

## Topics

### Data fields

Size

The number of bytes in this version check atom.

Type

The type of this atom.

Flags

A 32-bit integer.

Software package

A 32-bit Gestalt type specifying the software package to check for.

Version

An unsigned 32-bit integer containing either the minimum required version or the required value after a binary `AND` operation.

Mask

The mask for a binary `AND` operation on the Gestalt bitfield.

Check type

The type of check to perform, expressed as 16-bit integer.

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

Component detect atom ('rmcd')

A component detect atom specifies a QuickTime component, such as a particular video decompressor, required to play the movie.

Movie importer component flags

Flags that adjust the behavior of the movie import component.

Quality atom ('rmqu')

A quality atom describes the relative quality of a movie.

