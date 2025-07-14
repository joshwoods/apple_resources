

- AppKit
- NSPasteboard
-  detectedMetadata(for:) 

Instance Method

# detectedMetadata(for:)

Determines available metadata from the specified metadata types for the first pasteboard item, without notifying the user.

macOS 15.4+

``` source
func detectedMetadata(for keyPaths: Set>) async throws -> NSPasteboard.DetectedMetadata
```

## Parameters 

`keyPaths`  

The metadata types to detect on the pasteboard.

## Return Value

An object containing the metadata for the metadata types that were detected on the pasteboard.

## Discussion

Because this method only gives access to limited types of metadata and doesn’t allow the app to access the contents, the system doesn’t notify the user about reading the contents of the pasteboard.

For details about the metadata returned for each type, see `NSPasteboard.DetectedMetadata`.

