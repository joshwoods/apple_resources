

- QuickTime File Format
-  Track aperture mode dimensions atom ('tapt') 

Atom

# Track aperture mode dimensions atom ('tapt')

A container atom that stores information for video correction in the form of three required atoms.

## Mentioned in 

QuickTime File Format change log

## Overview

This atom is optionally included in the track atom. The type of the track aperture mode dimensions atom is `‘tapt’`.

The layout of a track aperture mode dimensions atom is as follows.

| Data | Type |
|----|----|
| Size | 4 bytes |
| Type = `'tapt'` | 4 bytes |
| Track clean aperture dimensions atom | `'clef'` |
| Track production aperture dimensions atom | `'prof'` |
| Track encoded pixels dimensions atom | `'enof'` |

## Topics

### Data fields

Size

A 32-bit integer that specifies the number of bytes in the track aperture mode dimensions atom.

Type

A 32-bit integer that identifies the atom type.

Track clean aperture dimensions atom

An atom that carries the pixel dimensions of the track’s clean aperture.

Track production aperture dimensions atom

An atom that carries the pixel dimensions of the track’s production aperture.

Track encoded pixels dimensions atom

An atom that carries the pixel dimensions of the track’s encoded pixels.

## See Also

### Track aperture mode dimension atoms

Track clean aperture dimensions atom ('clef')

An atom that carries the pixel dimensions of the track’s clean aperture.

Track production aperture dimensions atom ('prof')

An atom that carries the pixel dimensions of the track’s production aperture.

Track encoded pixels dimensions atom ('enof')

An atom that carries the pixel dimensions of the track’s encoded pixels.

