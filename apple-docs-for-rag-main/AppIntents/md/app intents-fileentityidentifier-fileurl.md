

- App Intents
- FileEntityIdentifier
-  fileURL 

Instance Property

# fileURL

A URL that locates a file saved to disk.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var fileURL: URL? { get async throws }
```

## Discussion

If the file is saved outside of your app’s container, make sure to surround access to file contents with `startAccessingSecurityScopedResource()` and `stopAccessingSecurityScopedResource()`.

