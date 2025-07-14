

- QuickTime File Format
-  Component detect atom ('rmcd') 

Atom

# Component detect atom ('rmcd')

A component detect atom specifies a QuickTime component, such as a particular video decompressor, required to play the movie.

## Overview

The component type, subtype, and other required attributes can be specified, as well as a minimum version. Multiple component detect atoms are allowed within a given reference movie descriptor atom. Applications should not attempt to play a movie unless at least the minimum versions of all required components are present.

## Topics

### Data fields

Size

The number of bytes in this component detect atom.

Type

The type of this atom.

Flags

A 32-bit integer.

Component description

A component description record.

Minimum version

An unsigned 32-bit integer containing the minimum required version of the specified component.

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

Movie importer component flags

Flags that adjust the behavior of the movie import component.

Quality atom ('rmqu')

A quality atom describes the relative quality of a movie.

