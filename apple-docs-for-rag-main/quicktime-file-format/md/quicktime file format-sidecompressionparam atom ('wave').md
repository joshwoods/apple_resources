

- QuickTime File Format
-  siDecompressionParam atom ('wave') 

Atom

# siDecompressionParam atom ('wave')

An atom that stores data specific to a given audio decompressor.

## Mentioned in 

Sound sample data

## Overview

The `siDecompressionParam` atom provides the ability to store data specific to a given audio decompressor in the `SoundDescription` record. As example, some audio decompression algorithms, such as Microsoft’s ADPCM, require a set of out-of-band values to configure the decompressor. These are stored in an atom of this type.

This atom contains other atoms with audio decompressor settings and is a required extension to the sound sample description for MPEG-4 audio. A `'wave'` chunk for `'mp4a'` typically contains (in order) at least a `'frma'` atom, an `'mp4a'` atom, an `'esds'` atom, and a Terminator atom ('0x00000000').

The contents of other `siDecompressionParam` atoms are dependent on the audio decompressor.

## Topics

### Data fields

Size

An unsigned 32-bit integer holding the size of the decompression parameters atom.

Type

An unsigned 32-bit field.

Extension atoms

Atoms containing the necessary out-of-band decompression parameters for the sound decompressor.

## See Also

### Extending sound sample descriptions

siSlopeAndIntercept atom

An atom that contains parameters relevant to a decompressor component.

Format atom ('frma')

An atom that shows the data format of the stored sound media.

Terminator atom ('0x00000000')

An atom that indicates the end of the sound description.

MPEG-4 elementary sound stream descriptor atom ('esds')

A required extension to the audio sample description for MPEG-4 audio.

Audio channel layout atom ('chan')

An optional extension to the sound sample description specifying audio channel layouts for sound media contained in QuickTime movies.

Subtitle follows track reference atom ('folw')

An atom that indicates a default subtitle track for a selected sound track.

