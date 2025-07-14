

- Media Toolbox
-  MTAudioProcessingTapCallbacks 

Structure

# MTAudioProcessingTapCallbacks

A structure that defines life cycle callbacks for an audio processing tap object.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
struct MTAudioProcessingTapCallbacks
```

## Overview

On 64-bit architectures, this struct contains misaligned function pointers. To avoid link-time issues, fill its function pointer fields by using assignment statements, rather than declaring them as global or static structs.

## Topics

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

var unprepare: MTAudioProcessingTapUnprepareCallback?

A callback to perform any necessary cleanup for previous preparation.

var process: MTAudioProcessingTapProcessCallback

A callback for processing the audio.

### Callback functions

typealias MTAudioProcessingTapInitCallback

An initialization callback function.

typealias MTAudioProcessingTapPrepareCallback

An audio processing preparation callback function.

typealias MTAudioProcessingTapProcessCallback

An audio processing callback function.

typealias MTAudioProcessingTapUnprepareCallback

An audio processing unpreparation callback function.

typealias MTAudioProcessingTapFinalizeCallback

A finalization callback function.

### Versions

var kMTAudioProcessingTapCallbacksVersion_0: Int32

An identifier for version 0 of the callbacks structure.

### Initializers

init(version: Int32, clientInfo: UnsafeMutableRawPointer?, init: MTAudioProcessingTapInitCallback?, finalize: MTAudioProcessingTapFinalizeCallback?, prepare: MTAudioProcessingTapPrepareCallback?, unprepare: MTAudioProcessingTapUnprepareCallback?, process: MTAudioProcessingTapProcessCallback)

## Relationships

### Conforms To

- BitwiseCopyable

