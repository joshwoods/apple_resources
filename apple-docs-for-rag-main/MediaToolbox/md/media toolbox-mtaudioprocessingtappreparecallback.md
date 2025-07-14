

- Media Toolbox
-  MTAudioProcessingTapPrepareCallback 

Type Alias

# MTAudioProcessingTapPrepareCallback

An audio processing preparation callback function.

iOS 6.0+iPadOS 6.0+Mac Catalyst 6.0+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
typealias MTAudioProcessingTapPrepareCallback = (MTAudioProcessingTap, CMItemCount, UnsafePointer) -> Void
```

## Parameters 

`tap`  

The processing tap.

`maxFrames`  

The maximum number of sample frames that can be requested of a processing tap at any one time. Typically this will be approximately 50 msec of audio (2048 samples @ 44.1kHz).

`processingFormat`  

The format in which the client will receive the audio data to be processed. This will always be the same sample rate as the client format and usually the same number of channels as the client format of the audio queue. (NOTE: the number of channels may be different in some cases if the client format has some channel count restrictions; for example, if the client provides 5.1 AAC, but the decoder can only produce stereo). The channel order, if the same as the client format, will be the same as the client channel order. If the channel count is changed, it will be to either 1 (mono) or 2 (stereo, in which case the first channel is left, the second right).

If the data is not in a convenient format for the client to process in, then the client should convert the data to and from that format. This is the most efficient mechanism to use, as the audio system may choose a format that is most efficient from its playback requirement.

## Overview

A preparation callback that is invoked when the underlying audio machinery is initialized.

The preparation callback should be where output buffers that will be returned by the ProcessingTapCallback are allocated (unless in-place processing is desired).

Note that the preparation callback can potentially be called multiple times over the lifetime of the tap object, if the client performs an operation that requires the underlying audio machinery to be torn down and rebuilt.

## See Also

### Callback functions

typealias MTAudioProcessingTapInitCallback

An initialization callback function.

typealias MTAudioProcessingTapProcessCallback

An audio processing callback function.

typealias MTAudioProcessingTapUnprepareCallback

An audio processing unpreparation callback function.

typealias MTAudioProcessingTapFinalizeCallback

A finalization callback function.

