

- AVFoundation
- AVSampleBufferGenerator
-  init(asset:timebase:) 

Initializer

# init(asset:timebase:)

Creates a new sample buffer generator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 10.10+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    asset: AVAsset,
    timebase: CMTimebase?
)
```

## Parameters 

`asset`  

The asset.

`timebase`  

If `NULL`, requests will be handled synchronously.

## Return Value

An initialized `AVSampleBufferGenerator` instance.

