

- AVFoundation
- AVMovie
-  data 

Instance Property

# data

A data object that contains the movie file’s data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
var data: Data? { get }
```

## Discussion

The value is `nil` if you didn’t initialize the movie with data.

## See Also

### Accessing Movie Information

var url: URL?

A URL to a QuickTime or ISO base media file.

