

- AVFoundation
- AVMutableMovie
-  init(settingsFrom:options:) 

Initializer

# init(settingsFrom:options:)

Creates a mutable movie object without tracks.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
init(
    settingsFrom movie: AVMovie?,
    options: [String : Any]? = nil
) throws
```

## Parameters 

`movie`  

A movie object that contains settings from an existing movie.

`options`  

A dictionary that contains key for specifying the movie object initialization. Currently, no keys are defined.

## Return Value

An `AVMutableMovie` object.

## Discussion

On initialization, the defaultMediaDataStorage property and any associated mediaDataStorage properties are set to `nil`. To create an `AVMutableMovie` from a file and then append sample buffers to any of its tracks, you must first set one of these properties to indicate where the sample data should be written.

## See Also

### Creating a Movie

init(url: URL, options: [String : Any]?, error: ()) throws

Creates a mutable movie object from a movie header stored in a QuickTime movie file of ISO base media file.

init(data: Data, options: [String : Any]?, error: ()) throws

Creates a mutable movie object from a movie stored in a data object.

