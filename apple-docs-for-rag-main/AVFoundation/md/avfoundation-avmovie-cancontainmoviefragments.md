

- AVFoundation
- AVMovie
-  canContainMovieFragments 

Instance Property

# canContainMovieFragments

A Boolean value that indicates whether fragments can extend the movie file.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+watchOS 6.0+

``` source
var canContainMovieFragments: Bool { get }
```

## Discussion

The value of this property is `YES` if an `mvex` box is present in the `moov` box. The `mvex` box is necessary to signal the possible presence of later `moof` boxes.

## See Also

### Determining Fragment Support

var containsMovieFragments: Bool

A Boolean value that indicates whether at least one movie fragment extends the movie file.

