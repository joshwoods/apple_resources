

- AVFoundation
- AVMovie
-  init(data:options:) 

Initializer

# init(data:options:)

Creates a movie object from a movie file’s data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
init(
    data: Data,
    options: [String : Any]? = nil
)
```

## Parameters 

`data`  

A data object that contains a movie header.

`options`  

A dictionary of options to use to initialize the movie.

## Discussion

Use this method to create movies from movie headers that aren’t stored in files, which can include movies that the pasteboard contains.

## See Also

### Creating a Movie

convenience init(url: URL)

Creates a movie that models the media at the specified URL.

init(url: URL, options: [String : Any]?)

Creates a movie object from a movie header stored in a QuickTime movie file of ISO base media file.

Initialization Options

Specify options to configure the initialization of a movie.

