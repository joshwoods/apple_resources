

- QuickTime File Format
-  Track clean aperture dimensions atom ('clef') 

Atom

# Track clean aperture dimensions atom ('clef')

An atom that carries the pixel dimensions of the track’s clean aperture.

## Overview

The type of the track clean aperture dimensions atom is `‘clef’`.

The layout of a track clean aperture dimensions atom is as follows.

| Data field | Bytes |
|----|----|
| Size | 4 |
| Type | 4 |
| Version | 1 |
| Flags | 3 |
| Width | 4 |
| Height | 4 |

## Topics

### Data fields

Size

A 32-bit integer that specifies the number of bytes in the atom.

Type

A 32-bit integer that identifies the atom type.

Version

A 1-byte specification of the version of this atom.

Flags

Three bytes that are reserved for the atom flags.

Width

A 32-bit fixed-point number that specifies the width of the track clean aperture in pixels.

Height

A 32-bit fixed-point number that specifies the height of the track clean aperture in pixels.

## See Also

### Track aperture mode dimension atoms

Track aperture mode dimensions atom ('tapt')

A container atom that stores information for video correction in the form of three required atoms.

Track production aperture dimensions atom ('prof')

An atom that carries the pixel dimensions of the track’s production aperture.

Track encoded pixels dimensions atom ('enof')

An atom that carries the pixel dimensions of the track’s encoded pixels.

