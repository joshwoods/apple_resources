

- AVFoundation
- AVMovie
-  url 

Instance Property

# url

A URL to a QuickTime or ISO base media file.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+watchOS 6.0+

``` source
var url: URL? { get }
```

## Discussion

The value is `nil` if you didn’t initialize the movie with a URL.

## See Also

### Accessing Movie Information

var data: Data?

A data object that contains the movie file’s data.

