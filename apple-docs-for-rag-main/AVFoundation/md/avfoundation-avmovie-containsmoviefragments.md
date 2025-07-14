

- AVFoundation
- AVMovie
-  containsMovieFragments 

Instance Property

# containsMovieFragments

A Boolean value that indicates whether at least one movie fragment extends the movie file.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
var containsMovieFragments: Bool { get }
```

## Discussion

This property is `YES` if canContainMovieFragments is `YES` and at least one `moof` box is present after the `moov` box.

## See Also

### Determining Fragment Support

var canContainMovieFragments: Bool

A Boolean value that indicates whether fragments can extend the movie file.

