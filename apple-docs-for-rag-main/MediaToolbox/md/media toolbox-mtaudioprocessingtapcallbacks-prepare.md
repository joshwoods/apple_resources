

- Media Toolbox
- MTAudioProcessingTapCallbacks
-  prepare 

Instance Property

# prepare

A callback to prepare the tap processor.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var prepare: MTAudioProcessingTapPrepareCallback?
```

## Discussion

Apps can use this callback to allocate memory buffers or perform other preparation. This field an be `NULL`.

Note

The system may call this function multiple times.

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

var unprepare: MTAudioProcessingTapUnprepareCallback?

A callback to perform any necessary cleanup for previous preparation.

var process: MTAudioProcessingTapProcessCallback

A callback for processing the audio.

