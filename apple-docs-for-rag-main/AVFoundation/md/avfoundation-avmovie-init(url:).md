

- AVFoundation
- AVMovie
-  init(url:) 

Initializer

# init(url:)

Creates a movie that models the media at the specified URL.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.10+visionOS 1.0+watchOS 6.0+

``` source
convenience init(url: URL)
```

## Parameters 

`url`  

A URL to a local, remote, or HTTP Live Streaming media resource.

## See Also

### Creating a Movie

init(url: URL, options: [String : Any]?)

Creates a movie object from a movie header stored in a QuickTime movie file of ISO base media file.

init(data: Data, options: [String : Any]?)

Creates a movie object from a movie file’s data.

Initialization Options

Specify options to configure the initialization of a movie.

