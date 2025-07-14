

- Media Toolbox
- MTAudioProcessingTapCallbacks
-  init 

Instance Property

# init

A callback to initialize the tap processor.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var `init`: MTAudioProcessingTapInitCallback?
```

## Discussion

This callback is called before MTAudioProcessingTapCreate(_:_:_:_:) returns. This field can be `NULL`.

## See Also

### Fields

var version: Int32

The version number of the structure.

var clientInfo: UnsafeMutableRawPointer?

App data that the system passes to the initialization callback.

var finalize: MTAudioProcessingTapFinalizeCallback?

A callback to perform any necessary cleanup.

var prepare: MTAudioProcessingTapPrepareCallback?

A callback to prepare the tap processor.

var unprepare: MTAudioProcessingTapUnprepareCallback?

A callback to perform any necessary cleanup for previous preparation.

var process: MTAudioProcessingTapProcessCallback

A callback for processing the audio.

