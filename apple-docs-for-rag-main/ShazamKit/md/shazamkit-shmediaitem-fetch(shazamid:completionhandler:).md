

- ShazamKit
- SHMediaItem
-  fetch(shazamID:completionHandler:) 

Type Method

# fetch(shazamID:completionHandler:)

Requests the media item for the song with the specified Shazam ID.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class func fetch(
    shazamID: String,
    completionHandler: @escaping (SHMediaItem?, (any Error)?) -> Void
)
```

``` source
class func fetch(shazamID: String) async throws -> SHMediaItem
```

## Parameters 

`shazamID`  

The Shazam ID of the song.

`completionHandler`  

The completion handler that the system calls with the result of the request.

This block takes the following parameters:

`mediaItem`  
A media item.

`error`  
An error object if a problem occurs when fetching the media item; otherwise, `nil`.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
class func fetch(shazamID: String) async throws -> SHMediaItem
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Working with Shazam music catalog media items

var webURL: URL?

A link to the Shazam Music catalog page that contains the full information for the song.

var shazamID: String?

The Shazam ID for the song.

