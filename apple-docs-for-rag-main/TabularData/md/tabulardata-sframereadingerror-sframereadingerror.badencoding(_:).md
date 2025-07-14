

- TabularData
- SFrameReadingError
-  SFrameReadingError.badEncoding(\_:) 

Case

# SFrameReadingError.badEncoding(\_:)

An error that indicates the scalable data frame contains bad data encoding.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
case badEncoding(String)
```

## Discussion

The associated value contains a description of the error.

## See Also

### Getting Error Information

case badArchive(String)

An error that indicates the scalable data frame directory’s archive file is corrupt.

case missingArchive

An error that indicates the scalable data frame directory is missing an archive file.

case missingColumn(String)

An error that indicates the scalable data frame is missing one of the requested columns.

case unsupportedArchive(String)

An error that indicates the scalable data frame contains an archive version or layout the framework doesn’t support.

case unsupportedLayout(String)

An error that indicates the scalable data frame contains an unsupported data layout.

case unsupportedType(Int)

An error that indicates the scalable data frame contains an unknown or unsupported data type.

