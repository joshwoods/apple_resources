

- AVFoundation
- AVMovie
-  is(compatibleWithFileType:) 

Instance Method

# is(compatibleWithFileType:)

Returns a Boolean value that indicates whether the system can create a movie header of the specified type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
func `is`(compatibleWithFileType fileType: AVFileType) -> Bool
```

## Parameters 

`fileType`  

A file type to test.

## Return Value

true if the movie only contains tracks whose media types are allowed by the specified file type; otherwise, false.

## See Also

### Creating and Writing Headers

func makeMovieHeader(fileType: AVFileType) throws -> Data

Creates a header for a movie for the specified file type.

func writeHeader(to: URL, fileType: AVFileType, options: AVMovieWritingOptions) throws

Writes the movie header to the specified URL.

struct AVMovieWritingOptions

A structure that defines options to control the writing of a movie header to a destination URL.

