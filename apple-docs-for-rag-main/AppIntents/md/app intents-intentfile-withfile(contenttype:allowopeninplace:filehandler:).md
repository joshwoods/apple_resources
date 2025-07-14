

- App Intents
- IntentFile
-  withFile(contentType:allowOpenInPlace:fileHandler:) 

Instance Method

# withFile(contentType:allowOpenInPlace:fileHandler:)

Requests an `IntentFile` representation as a file url.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func withFile(
    contentType: UTType,
    allowOpenInPlace: Bool = false,
    fileHandler: @escaping (URL, Bool) async throws -> Result
) async throws -> Result
```

## Parameters 

`contentType`  

A content type of the returned data.

`allowOpenInPlace`  

Whether the file should be opened in place, if possible.

`fileHandler`  

A closure that accepts the file URL as a parameter. The file is written to a temporary destination and removed right after the closure returns.

## Discussion

If the file is not opened in place, the system removes it after the fileHandler closure returns.

```
let image = try await intentFile.withFile(contentType: .png) { url, _ in
    let data = try Data(contentsOf: url)
    return CGImage(pngData: data)
}
```

