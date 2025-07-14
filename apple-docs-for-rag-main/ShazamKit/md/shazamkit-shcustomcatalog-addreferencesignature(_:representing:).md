

- ShazamKit
- SHCustomCatalog
-  addReferenceSignature(\_:representing:) 

Instance Method

# addReferenceSignature(\_:representing:)

Adds a reference signature and its associated metadata to a catalog.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func addReferenceSignature(
    _ signature: SHSignature,
    representing mediaItems: [SHMediaItem]
) throws
```

## Parameters 

`signature`  

The reference signature for the audio recording.

`mediaItems`  

The metadata for the recording.

## Discussion

Note

This system ignores calls to `addReferenceSignature(_:representing:)` after adding the catalog to an `SHSession`.

