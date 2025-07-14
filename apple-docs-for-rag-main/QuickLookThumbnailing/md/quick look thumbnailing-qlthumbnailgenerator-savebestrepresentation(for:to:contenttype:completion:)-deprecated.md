

- Quick Look Thumbnailing
- QLThumbnailGenerator
-  saveBestRepresentation(for:to:contentType:completion:) Deprecated

Instance Method

# saveBestRepresentation(for:to:contentType:completion:)

Saves the best representation of thumbnail for a specific request to the specified URL.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func saveBestRepresentation(
    for request: QLThumbnailGenerator.Request,
    to fileURL: URL,
    contentType: String,
    completion completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func saveBestRepresentation(
    for request: QLThumbnailGenerator.Request,
    to fileURL: URL,
    contentType: String
) async throws
```

## Parameters 

`request`  

The request that you used to generate a thumbnail.

`fileURL`  

The destination to which you save the generated thumbnail.

`contentType`  

The content type of the thumbnail image that you want to save. Use a type that is supported by CGImageDestination, such as `kUTTypePNG` or `kUTTypeJPEG`.

`completionHandler`  

The handler to call when saving the thumbnail to disk.

`error`  
An error object that indicates why saving a thumbnail image failed, or `nil` if saving the thumbnail succeeded.

## Mentioned in 

Creating Quick Look Thumbnails to Preview Files in Your App

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func saveBestRepresentation(for request: QLThumbnailGenerator.Request, to fileURL: URL, contentType: String) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Creating high-quality thumbnails often involves compressing a CGImage as a `PNG` or `JPEG` file in-process. This task requires more resources than are available in resource-constrained environments such as File Provider Extensions.

Use this method to create and save the thumbnail image outside of your process as it doesn’t impose the same constraints on memory usage.

