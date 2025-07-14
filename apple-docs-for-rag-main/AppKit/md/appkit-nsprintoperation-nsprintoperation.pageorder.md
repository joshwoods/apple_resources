

- AppKit
- NSPrintOperation
-  NSPrintOperation.PageOrder 

Enumeration

# NSPrintOperation.PageOrder

Constants that specify the page order.

macOS

``` source
enum PageOrder
```

## Overview

These constants are used by pageOrder and pageOrder.

## Topics

### Constants

case ascendingPageOrder

Ascending (back to front) page order.

case descendingPageOrder

Descending (front to back) page order.

case specialPageOrder

The spooler does not rearrange pages—they are printed in the order received by the spooler.

case unknownPageOrder

No page order specified.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing Page Information

var currentPage: Int

The current page number being printed.

var pageRange: NSRange

The range of pages associated with the print operation.

var pageOrder: NSPrintOperation.PageOrder

The print order for the pages of the operation.

