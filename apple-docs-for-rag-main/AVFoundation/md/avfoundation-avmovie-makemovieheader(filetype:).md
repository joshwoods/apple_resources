

- AVFoundation
- AVMovie
-  makeMovieHeader(fileType:) 

Instance Method

# makeMovieHeader(fileType:)

Creates a header for a movie for the specified file type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
func makeMovieHeader(fileType: AVFileType) throws -> Data
```

## Parameters 

`fileType`  

A UTI that indicates the specific file format for the movie header.

## Return Value

An NSData object containing the movie header.

## Discussion

The created movie header is a pure reference movie, with no base URL, suitable for use on the pasteboard.

## See Also

### Creating and Writing Headers

func `is`(compatibleWithFileType: AVFileType) -> Bool

Returns a Boolean value that indicates whether the system can create a movie header of the specified type.

func writeHeader(to: URL, fileType: AVFileType, options: AVMovieWritingOptions) throws

Writes the movie header to the specified URL.

struct AVMovieWritingOptions

A structure that defines options to control the writing of a movie header to a destination URL.

