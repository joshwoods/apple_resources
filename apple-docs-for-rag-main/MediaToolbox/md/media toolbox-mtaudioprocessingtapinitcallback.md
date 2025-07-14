

- Media Toolbox
-  MTAudioProcessingTapInitCallback 

Type Alias

# MTAudioProcessingTapInitCallback

An initialization callback function.

iOS 6.0+iPadOS 6.0+Mac Catalyst 6.0+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
typealias MTAudioProcessingTapInitCallback = (MTAudioProcessingTap, UnsafeMutableRawPointer?, UnsafeMutablePointer) -> Void
```

## Parameters 

`tap`  

The processing tap.

`clientInfo`  

The client data of the processing tap passed in callbacks struct in MTAudioProcessingTapCreate().

`tapStorageOut`  

Additional client data. The intent is for clients to allocate a block of memory for use within their custom MTAudioProcessingTap implementation that will be freed when the finalize callback is invoked. This argument is optional.

## Overview

An init callback that is invoked when MTAudioProcessingTapCreate() is called. The init callback is always balanced by a finalize callback when the MTAudioProcessingTap object is released.

## See Also

### Callback functions

typealias MTAudioProcessingTapPrepareCallback

An audio processing preparation callback function.

typealias MTAudioProcessingTapProcessCallback

An audio processing callback function.

typealias MTAudioProcessingTapUnprepareCallback

An audio processing unpreparation callback function.

typealias MTAudioProcessingTapFinalizeCallback

A finalization callback function.

