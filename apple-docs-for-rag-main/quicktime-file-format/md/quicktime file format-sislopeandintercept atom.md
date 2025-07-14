

- QuickTime File Format
-  siSlopeAndIntercept atom 

Atom

# siSlopeAndIntercept atom

An atom that contains parameters relevant to a decompressor component.

## Overview

Note

The siSlopeAndIntercept atom is deprecated in the QuickTime file format. The information that follows documents existing content containing this atom and should not be used for new development.

The siSlopeAndIntercept atom contains `slope`, `intercept`, `minClip`, and `maxClip` parameters relevant to a decompressor component.

At runtime, the contents of the type `siSlopeAndIntercept` and `siDecompressorSettings` atoms are provided to the decompressor component through the standard `SetInfo` mechanism of the Sound Manager.

```
struct SoundSlopeAndInterceptRecord {
    Float64                 slope;
    Float64                 intercept;
    Float64                 minClip;
    Float64                 maxClip;
};
typedef struct SoundSlopeAndInterceptRecord SoundSlopeAndInterceptRecord;
```

## Topics

### Data fields

Slope

Intercept

minClip

maxClip

## See Also

### Extending sound sample descriptions

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

Subtitle follows track reference atom ('folw')

An atom that indicates a default subtitle track for a selected sound track.

