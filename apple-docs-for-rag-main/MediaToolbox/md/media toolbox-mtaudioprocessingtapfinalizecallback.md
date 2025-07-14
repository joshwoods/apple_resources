

- Media Toolbox
-  MTAudioProcessingTapFinalizeCallback 

Type Alias

# MTAudioProcessingTapFinalizeCallback

A finalization callback function.

iOS 6.0+iPadOS 6.0+Mac Catalyst 6.0+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
typealias MTAudioProcessingTapFinalizeCallback = (MTAudioProcessingTap) -> Void
```

## Parameters 

`tap`  

The processing tap.

## Overview

This callback is called when it is safe to free any buffers or other state associated with the tap. This callback will be called exactly once when the MTAudioProcessingTap object is finalized. If tapStorage was allocated in the init callback, it should be freed here.

## See Also

### Callback functions

typealias MTAudioProcessingTapInitCallback

An initialization callback function.

typealias MTAudioProcessingTapPrepareCallback

An audio processing preparation callback function.

typealias MTAudioProcessingTapProcessCallback

An audio processing callback function.

typealias MTAudioProcessingTapUnprepareCallback

An audio processing unpreparation callback function.

