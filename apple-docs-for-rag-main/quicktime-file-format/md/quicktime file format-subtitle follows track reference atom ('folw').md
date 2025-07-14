

- QuickTime File Format
-  Subtitle follows track reference atom ('folw') 

Atom

# Subtitle follows track reference atom ('folw')

An atom that indicates a default subtitle track for a selected sound track.

## Overview

Sound tracks can have a track reference of type `'folw'` (for “follows”) to a single subtitle track from among the subtitle tracks in the same alternate group; this subtitle track should be considered the default to select if the sound track is selected. Use this only if compatibility between language tags is not possible for some reason making it impossible to otherwise select a default track. See Preparing sound and subtitle alternate groups for use with Apple devices for related information.

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

Audio channel layout atom ('chan')

An optional extension to the sound sample description specifying audio channel layouts for sound media contained in QuickTime movies.

