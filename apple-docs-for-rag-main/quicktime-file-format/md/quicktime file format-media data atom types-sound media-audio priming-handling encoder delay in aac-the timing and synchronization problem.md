

- QuickTime File Format
- Media data atom types
- Sound media
- Audio priming-handling encoder delay in AAC
-  The timing and synchronization problem 

Article

# The timing and synchronization problem

Trim the silent priming samples to preserve correct synchronization.

## Overview

If an audio playback system attempting to synchronize AAC encoded audio and video does not compensate for encoder delay (that is, does not discard the silent priming samples), the audio and video will be out of synchronization. In the example above, it will be off by 2112 samples—The audio will be 2112 samples behind the video because the first real audio sample is actually the 2113th sample after the beginning of the decoded PCM data.

Therefore, a playback system must trim the silent priming samples to preserve correct synchronization. This trimming by the playback system should be done in two places:

- When playback first begins

- When the playback position is moved to another location. For example, the user skips ahead or back to another part of the media and begins playback from that new location.

## See Also

### Handling encoder delay

AAC encoding background

AAC requires data beyond the source PCM audio samples in order to correctly encode and decode audio samples due to the nature of the encoding algorithm.

Historical solution for implicit encoder delay

Implicit encoder delay uses the most common delay of 2112 audio samples.

Using track structures to represent encoder delay explicitly

Represent encoder delay explicitly with an edit list atom and sample group structures.

Representing encoder delay explicitly

Review an example that represents the temporal position of 5 seconds of 48kHz PCM audio encoded in a 48kHz AAC sound track.

Representing encoder delay with track structures

Use sample group structures to represent encoder delay for AAC sound tracks.

