

- AVFoundation
- AVMutableMovie
-  init(data:options:error:) 

Initializer

# init(data:options:error:)

Creates a mutable movie object from a movie stored in a data object.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
init(
    data: Data,
    options: [String : Any]? = nil,
    error: ()
) throws
```

## Parameters 

`data`  

An `NSData` object that contains a movie header.

`options`  

A dictionary that contains key for specifying the movie object initialization. Currently, no keys are defined.

## Return Value

An `AVMutableMovie` object.

## Discussion

On initialization, the defaultMediaDataStorage property and any associated mediaDataStorage properties are set to `nil`. To create an `AVMutableMovie` from a file and then append sample buffers to any of its tracks, you must first set one of these properties to indicate where the sample data should be written.

Use this method to create movies from movie headers that are not stored in files, which can include movies on the pasteboard.

## See Also

### Creating a Movie

init(url: URL, options: [String : Any]?, error: ()) throws

Creates a mutable movie object from a movie header stored in a QuickTime movie file of ISO base media file.

init(settingsFrom: AVMovie?, options: [String : Any]?) throws

Creates a mutable movie object without tracks.

