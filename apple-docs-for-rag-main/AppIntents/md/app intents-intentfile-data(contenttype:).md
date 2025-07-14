

- App Intents
- IntentFile
-  data(contentType:) 

Instance Method

# data(contentType:)

Requests an `IntentFile` representation as binary data of the requested content type if possible.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func data(contentType: UTType) async throws -> Data
```

## Parameters 

`contentType`  

A content type of the returned data.

## Discussion

If the `IntentFile` is backed by a file `URL`, this might cause loading the entire file contents into memory.

