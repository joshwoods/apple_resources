

- AVFoundation
-  AVMovieWritingOptions 

Structure

# AVMovieWritingOptions

A structure that defines options to control the writing of a movie header to a destination URL.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
struct AVMovieWritingOptions
```

## Topics

### Writing Options

static var addMovieHeaderToDestination: AVMovieWritingOptions

The new movie header overwrites any existing movie header.

static var truncateDestinationToMovieHeaderOnly: AVMovieWritingOptions

The movie header overwrites all existing data and creates a pure reference movie file.

### Initializers

init(rawValue: UInt)

Creates a movie writing options structure.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Creating and Writing Headers

func `is`(compatibleWithFileType: AVFileType) -> Bool

Returns a Boolean value that indicates whether the system can create a movie header of the specified type.

func makeMovieHeader(fileType: AVFileType) throws -> Data

Creates a header for a movie for the specified file type.

func writeHeader(to: URL, fileType: AVFileType, options: AVMovieWritingOptions) throws

Writes the movie header to the specified URL.

