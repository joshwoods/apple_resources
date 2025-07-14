

- TabularData
- SFrameReadingError
-  SFrameReadingError.unsupportedType(\_:) 

Case

# SFrameReadingError.unsupportedType(\_:)

An error that indicates the scalable data frame contains an unknown or unsupported data type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
case unsupportedType(Int)
```

## Discussion

The associated value contains the unknown data type identifier.

## See Also

### Getting Error Information

case badArchive(String)

An error that indicates the scalable data frame directory’s archive file is corrupt.

case badEncoding(String)

An error that indicates the scalable data frame contains bad data encoding.

case missingArchive

An error that indicates the scalable data frame directory is missing an archive file.

case missingColumn(String)

An error that indicates the scalable data frame is missing one of the requested columns.

case unsupportedArchive(String)

An error that indicates the scalable data frame contains an archive version or layout the framework doesn’t support.

case unsupportedLayout(String)

An error that indicates the scalable data frame contains an unsupported data layout.

