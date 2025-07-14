

- QuickTime File Format
-  Terminator atom ('0x00000000') 

Atom

# Terminator atom ('0x00000000')

An atom that indicates the end of the sound description.

## Mentioned in 

Sound sample data

## Overview

This atom is present to indicate the end of the sound description. It contains no data, and has a type field of zero (`0x00000000`) instead of a four-character code.

## Topics

### Data fields

Size

An unsigned 32-bit integer holding the size of the decompression parameters atom.

Type

An unsigned 32-bit integer.

## See Also

### Extending sound sample descriptions

siSlopeAndIntercept atom

An atom that contains parameters relevant to a decompressor component.

siDecompressionParam atom ('wave')

An atom that stores data specific to a given audio decompressor.

Format atom ('frma')

An atom that shows the data format of the stored sound media.

MPEG-4 elementary sound stream descriptor atom ('esds')

A required extension to the audio sample description for MPEG-4 audio.

Audio channel layout atom ('chan')

An optional extension to the sound sample description specifying audio channel layouts for sound media contained in QuickTime movies.

Subtitle follows track reference atom ('folw')

An atom that indicates a default subtitle track for a selected sound track.

