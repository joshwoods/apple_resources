

- Media Toolbox
- MTAudioProcessingTapCallbacks
-  unprepare 

Instance Property

# unprepare

A callback to perform any necessary cleanup for previous preparation.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var unprepare: MTAudioProcessingTapUnprepareCallback?
```

## Discussion

This field can be `NULL`.

## See Also

### Fields

var version: Int32

The version number of the structure.

var clientInfo: UnsafeMutableRawPointer?

App data that the system passes to the initialization callback.

var `init`: MTAudioProcessingTapInitCallback?

A callback to initialize the tap processor.

var finalize: MTAudioProcessingTapFinalizeCallback?

A callback to perform any necessary cleanup.

var prepare: MTAudioProcessingTapPrepareCallback?

A callback to prepare the tap processor.

var process: MTAudioProcessingTapProcessCallback

A callback for processing the audio.

