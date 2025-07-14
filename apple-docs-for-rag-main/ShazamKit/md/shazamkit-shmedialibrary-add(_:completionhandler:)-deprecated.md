

- ShazamKit
- SHMediaLibrary
-  add(\_:completionHandler:) Deprecated

Instance Method

# add(\_:completionHandler:)

Adds an array of songs to the user’s Shazam library.

iOS 15.0–18.0DeprecatediPadOS 15.0–18.0DeprecatedMac Catalyst 15.0–18.0DeprecatedmacOS 12.0–15.0DeprecatedtvOS 15.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 8.0–11.0Deprecated

``` source
func add(
    _ mediaItems: [SHMediaItem],
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func add(_ mediaItems: [SHMediaItem]) async throws
```

Deprecated

Use SHLibrary instead

## Parameters 

`mediaItems`  

An array of media items that represents the songs to add to the library.

`completionHandler`  

The system calls this completion block after adding the media items to the library.

This block takes the following parameters:

`error`  
An error object if a problem occurs when adding any item; otherwise, `nil`.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func add(_ mediaItems: [SHMediaItem]) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Saving a song to the user’s Shazam library also saves the following media item properties and their associated values:

- shazamID

- title

- subtitle, or artist if the subtitle is unavailable

Note

Saving to the user’s Shazam library works only for songs with a valid shazamID.

## See Also

### Adding a matched song to the library

class var `default`: SHMediaLibrary

An instance of the user’s default Shazam library.

Deprecated

