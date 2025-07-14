

- Media Toolbox
- MTAudioProcessingTapCallbacks
-  version 

Instance Property

# version

The version number of the structure.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var version: Int32
```

## Discussion

The value is passed as a parameter to MTAudioProcessingTapCreate(_:_:_:_:). It must be set to kMTAudioProcessingTapCallbacksVersion_0.

## See Also

### Fields

var clientInfo: UnsafeMutableRawPointer?

App data that the system passes to the initialization callback.

var `init`: MTAudioProcessingTapInitCallback?

A callback to initialize the tap processor.

var finalize: MTAudioProcessingTapFinalizeCallback?

A callback to perform any necessary cleanup.

var prepare: MTAudioProcessingTapPrepareCallback?

A callback to prepare the tap processor.

var unprepare: MTAudioProcessingTapUnprepareCallback?

A callback to perform any necessary cleanup for previous preparation.

var process: MTAudioProcessingTapProcessCallback

A callback for processing the audio.

