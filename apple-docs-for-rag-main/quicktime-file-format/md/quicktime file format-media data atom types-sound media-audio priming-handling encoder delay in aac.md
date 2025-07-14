

- QuickTime File Format
- Media data atom types
- Sound media
-  Audio priming-handling encoder delay in AAC 

# Audio priming-handling encoder delay in AAC

Position a source audio signal in a sound track to handle encoder delay.

## Overview

This section describes temporal positioning of a source audio signal after AAC encoding into a sound track for QuickTime media files. The mechanisms described here are specified in ISO MPEG-4 standards (ISO/IEC 14496-12, 2008) and are used here with additional constraints.

Note

AAC implementations typically represent 1024 PCM audio samples in one AAC packet (synonymous in this context with a QuickTime media sample, and also referred to in ISO documents as an “access unit”). The terms “sample” and “audio sample” in this appendix are used to refer to PCM samples. For the encoded audio data, the terms “AAC packet” and QuickTime “media sample” are used.

## Topics

### Handling encoder delay

AAC encoding background

AAC requires data beyond the source PCM audio samples in order to correctly encode and decode audio samples due to the nature of the encoding algorithm.

The timing and synchronization problem

Trim the silent priming samples to preserve correct synchronization.

Historical solution for implicit encoder delay

Implicit encoder delay uses the most common delay of 2112 audio samples.

Using track structures to represent encoder delay explicitly

Represent encoder delay explicitly with an edit list atom and sample group structures.

Representing encoder delay explicitly

Review an example that represents the temporal position of 5 seconds of 48kHz PCM audio encoded in a 48kHz AAC sound track.

Representing encoder delay with track structures

Use sample group structures to represent encoder delay for AAC sound tracks.

## See Also

### Storing audio data

Sound sample descriptions

A sound sample description contains information that defines how to interpret sound media data.

Sound sample description extensions

Extend sound sample descriptions by appending other atoms.

Sound sample data

Sound sample formats that QuickTime supports.

