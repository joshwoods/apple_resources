

- QuickTime File Format
- Media data atom types
- Sound media
- Audio priming-handling encoder delay in AAC
-  AAC encoding background 

Article

# AAC encoding background

AAC requires data beyond the source PCM audio samples in order to correctly encode and decode audio samples due to the nature of the encoding algorithm.

## Overview

AAC requires data beyond the source PCM audio samples in order to correctly encode and decode audio samples due to the nature of the encoding algorithm. AAC encoding uses a transform over consecutive sets of 2048 audio samples, applied every 1024 audio samples (overlapped). For correct audio to be decoded, both transforms for any period of 1024 audio samples are needed. For this reason, encoders add at least 1024 samples of silence before the first ‘true’ audio sample, and often add more. This is called variously “priming”, “priming samples”, or “encoder delay”. A couple of definitions for use in this discussion:

- *Encoder delay* is the delay incurred during encoding to produce properly formed, encoded audio packets. It typically refers to the number of silent media samples (priming samples) added to the front of an AAC encoded bitstream.

- *Decoder delay* is the number of “pre-roll” audio samples required to reproduce an encoded source audio signal for a given time index. For AAC this number is typically 1024 and is algorithmically based. This is in contrast to encoder delay which is determined by the encoder and encoding configuration used. However, decoder delay establishes the minimum encoder delay possible (that is, 1024 for AAC).

The common practice is to propagate the encoder delay in the AAC bitstream. When these audio packets are then decoded back to the PCM domain, the source waveform represented will be offset in its entirety by this encoder delay amount. Since encoded audio packets hold a fixed number of audio samples (for instance, 1024 samples) additional trailing or ‘remainder’ silent samples following the last source sample are required so as to pad the final audio packet to the required length.

The following figure gives an example of a typical encoded AAC audio bitstream. The upper portion of the illustration represents the AAC encoded domain with equal-sized AAC packets, the lower portion represents the PCM sample domain:

The source audio to be encoded, shown as the red waveform, is 5389 samples long. You can see how it is represented with the blue priming and remainder samples against the fixed size access units – AAC packets – drawn above it.

This data will be represented in 8 AAC packets, where each packet represents 1024 audio samples. The total duration represented by these 8 AAC packets is 8192 audio samples (note that this is longer than the duration of the source audio).

The result breaks down into the following values:

- 2112 priming samples at the start—Required to correctly encode the start of the audio.

- 5389 samples of actual audio.

- 691 remainder samples—Required to pad out to the AAC packet size.

Therefore, to correctly extract the original 5389 samples of source audio, the first 2112 samples of priming and the last 691 samples of the remainder must be removed.

- 8192 - 2112 - 691 = 5389 original source samples.

## See Also

### Handling encoder delay

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

