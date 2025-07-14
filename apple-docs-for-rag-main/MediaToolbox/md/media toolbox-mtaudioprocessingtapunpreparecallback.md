

- Media Toolbox
-  MTAudioProcessingTapUnprepareCallback 

Type Alias

# MTAudioProcessingTapUnprepareCallback

An audio processing unpreparation callback function.

iOS 6.0+iPadOS 6.0+Mac Catalyst 6.0+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
typealias MTAudioProcessingTapUnprepareCallback = (MTAudioProcessingTap) -> Void
```

## Parameters 

`tap`  

The processing tap.

## Overview

The unpreparation callback is invoked when the underlying audio machinery stops calling the process callback.

Preparation and unpreparation callbacks are always paired.

Process callbacks will only ever be called after the prepare callback returns, and before unprepare is called.

## Topics

### Flags

typealias MTAudioProcessingTapCreationFlags

Flags to use when creating audio processing taps.

## See Also

### Callback functions

typealias MTAudioProcessingTapInitCallback

An initialization callback function.

typealias MTAudioProcessingTapPrepareCallback

An audio processing preparation callback function.

typealias MTAudioProcessingTapProcessCallback

An audio processing callback function.

typealias MTAudioProcessingTapFinalizeCallback

A finalization callback function.

