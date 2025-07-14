

- QuickTime File Format
- Media data atom types
- Sound media
-  Sound sample description extensions 

API Collection

# Sound sample description extensions

Extend sound sample descriptions by appending other atoms.

## Overview

All extensions to the SoundDescription record are made using atoms. That means one or more atoms can be appended to the end of the SoundDescription record using the standard \[size, type\] mechanism used throughout the QuickTime movie architecture. Extensions were first added with sound sample description v1.

To illustrate this, for sound sample description v1, the extensions are added by following the last field of the struct with QuickTime atoms. The struct implementation looks like this:

```
struct SoundDescriptionV1 {
    // original fields
    SoundDescription    desc;
    // fixed compression ratio information
    unsigned long   samplesPerPacket;
    unsigned long   bytesPerPacket;
    unsigned long   bytesPerFrame;
    unsigned long   bytesPerSample;
    // optional, additional atom-based fields --
    // ([long size, long type, some data], repeat)
};
```

Version 2 of the sound sample description maintains the same mechanism for the addition of extensions. In the sound sample description v2 structure, the `sizeOfStructOnly` field value provides the offset to the extensions.

## Topics

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

Subtitle follows track reference atom ('folw')

An atom that indicates a default subtitle track for a selected sound track.

## See Also

### Storing audio data

Sound sample descriptions

A sound sample description contains information that defines how to interpret sound media data.

Sound sample data

Sound sample formats that QuickTime supports.

Audio priming-handling encoder delay in AAC

Position a source audio signal in a sound track to handle encoder delay.

