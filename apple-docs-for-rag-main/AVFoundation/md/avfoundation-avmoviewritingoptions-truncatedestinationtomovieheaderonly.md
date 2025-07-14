

- AVFoundation
- AVMovieWritingOptions
-  truncateDestinationToMovieHeaderOnly 

Type Property

# truncateDestinationToMovieHeaderOnly

The movie header overwrites all existing data and creates a pure reference movie file.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
static var truncateDestinationToMovieHeaderOnly: AVMovieWritingOptions { get }
```

## Discussion

Creates a file type box at the beginning of the destination file.

## See Also

### Writing Options

static var addMovieHeaderToDestination: AVMovieWritingOptions

The new movie header overwrites any existing movie header.

