

- QuickTime File Format
-  Audio channel layout atom ('chan') 

Atom

# Audio channel layout atom ('chan')

An optional extension to the sound sample description specifying audio channel layouts for sound media contained in QuickTime movies.

## Overview

This atom is an optional extension to the sound sample description specifying audio channel layouts for sound media contained in QuickTime movies. It is a full atom followed by a big-endian audio channel layout structure as defined by Apple’s Core Audio framework. Audio channel layouts can be applied to both compressed and uncompressed sound formats.

Note

Audio channel layouts with more than two channels per track require implementation with a version 2 sound sample description.

## Topics

### Data fields

Size

An unsigned 32-bit integer holding the size of the audio channel layout atom.

Type

An unsigned 32-bit field.

Version

A 1-byte specification of the version of the audio channel layout atom.

Flags

A 3-byte space for audio channel layout flags.

Audio channel layout

An audio channel layout structure.

## See Also

### Extending sound sample descriptions

siSlopeAndIntercept atom

An atom that contains parameters relevant to a decompressor component.

siDecompressionParam atom ('wave')

An atom that stores data specific to a given audio decompressor.

Format atom ('frma')

An atom that shows the data format of the stored sound media.

Terminator atom ('0x00000000')

An atom that indicates the end of the sound description.

MPEG-4 elementary sound stream descriptor atom ('esds')

A required extension to the audio sample description for MPEG-4 audio.

Subtitle follows track reference atom ('folw')

An atom that indicates a default subtitle track for a selected sound track.

