

- AppKit
- NSPrintInfo
-  NSPrintInfo.PaginationMode 

Enumeration

# NSPrintInfo.PaginationMode

Constants that specify the different ways in which an image is divided into pages.

macOS

``` source
enum PaginationMode
```

## Overview

These constants are used by horizontalPagination and verticalPagination.

## Topics

### Constants

case automatic

case fit

case clip

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Pagination

var horizontalPagination: NSPrintInfo.PaginationMode

The horizontal pagination mode.

var verticalPagination: NSPrintInfo.PaginationMode

The vertical pagination to the specified mode.

