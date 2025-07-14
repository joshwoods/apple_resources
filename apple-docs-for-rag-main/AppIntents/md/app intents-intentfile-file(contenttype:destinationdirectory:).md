

- App Intents
- IntentFile
-  file(contentType:destinationDirectory:) 

Instance Method

# file(contentType:destinationDirectory:)

Requests an `IntentFile` representation as a file url.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func file(
    contentType: UTType,
    destinationDirectory: URL? = nil
) async throws -> (fileURL: URL, openedInPlace: Bool)
```

## Parameters 

`contentType`  

A content type of the returned data.

`destinationDirectory`  

The directory the file should be copied to, if no directory is provided the file is opened in place.

## Discussion

If a destination directory is not given the file is opened in place, falling back to a temporary directory if this fails. If the file is not opened in place and a destination directory is used it is the caller’s responsibility to remove the file.

