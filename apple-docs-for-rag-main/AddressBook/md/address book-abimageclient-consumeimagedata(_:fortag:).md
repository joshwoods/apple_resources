

- Address Book
- ABImageClient
-  consumeImageData(\_:forTag:) 

Instance Method

# consumeImageData(\_:forTag:)

Gets the image data for the given tag that was initiated by an asynchronous fetch.

macOS 10.10+

``` source
func consumeImageData(
    _ data: Data!,
    forTag tag: Int
)
```

**Required**

## Parameters 

`data`  

A pointer to a data object that will be set to an `NSImage`/QuickTime compatible format, or `nil` if no image could be found.

You can use this image data with the `initWithData:` method of the `NSImage` class.

`tag`  

The tag returned from a previous call to the `ABPerson` beginLoadingImageData(for:) method.

## Discussion

In the case of a multithreaded application, this method is always called on the main thread.

