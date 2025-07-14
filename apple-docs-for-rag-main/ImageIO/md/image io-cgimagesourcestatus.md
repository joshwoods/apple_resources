

- Image I/O
-  CGImageSourceStatus 

Enumeration

# CGImageSourceStatus

The set of status values for images and image sources.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum CGImageSourceStatus
```

## Overview

The CGImageSourceGetStatus(_:) and CGImageSourceGetStatusAtIndex(_:_:) functions return these values.

## Topics

### Status Values

case statusUnexpectedEOF

The end of the file occurred unexpectedly.

case statusInvalidData

The data is not valid.

case statusUnknownType

The image is an unknown type.

case statusReadingHeader

The image source is reading the header.

case statusIncomplete

The operation is not complete

case statusComplete

The operation is complete.

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the Image Status

func CGImageSourceGetStatus(CGImageSource) -> CGImageSourceStatus

Return the status of an image source.

func CGImageSourceGetStatusAtIndex(CGImageSource, Int) -> CGImageSourceStatus

Returns the current status of an image at the specified location in the image source.

