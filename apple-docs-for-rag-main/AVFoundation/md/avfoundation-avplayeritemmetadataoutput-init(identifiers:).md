

- AVFoundation
- AVPlayerItemMetadataOutput
-  init(identifiers:) 

Initializer

# init(identifiers:)

Creates an instance of AVPlayerItemMetadataOutput.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
init(identifiers: [String]?)
```

## Parameters 

`identifiers`  

A array of metadata identifiers indicating the metadata items that the output should provide.

## Return Value

An AVPlayerItemMetadataOutput instance.

## Discussion

Pass `nil` to receive all of the timed metadata from all enabled `AVPlayerItemTracks` that carry timed metadata.

