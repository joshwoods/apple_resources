

- AVFoundation
- AVMovie
-  init(url:options:) 

Initializer

# init(url:options:)

Creates a movie object from a movie header stored in a QuickTime movie file of ISO base media file.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+watchOS 6.0+

``` source
init(
    url URL: URL,
    options: [String : Any]? = nil
)
```

## Parameters 

`URL`  

A URL that points to a file containing a movie header.

`options`  

A dictionary of options to use to initialize the movie.

## Discussion

Upon creation, the values of the defaultMediaDataStorage property and any associated mediaDataStorage properties are `nil`.

## See Also

### Creating a Movie

convenience init(url: URL)

Creates a movie that models the media at the specified URL.

init(data: Data, options: [String : Any]?)

Creates a movie object from a movie file’s data.

Initialization Options

Specify options to configure the initialization of a movie.

