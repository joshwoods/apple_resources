

- UIKit
-  UIPrinterDestination 

Class

# UIPrinterDestination

A description of a single printer.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+visionOS 1.0+

``` source
@MainActor
class UIPrinterDestination
```

## Overview

You can use `UIPrinterDestination` to describe a printer so that it populates in a UIPrinterPickerController when the printer’s capabilities match the print-job attributes. `UIPrinterDestination` requires a URL to locate the printer. You can include an optional display name that populates in the user interface and a TXT record to detail the printer’s additional features.

## Topics

### Creating a printer destination

init(url: URL)

Creates a printer destination with the specified address.

### Describing the printer

var displayName: String?

A human-readable string that displays the name of a printer.

var txtRecord: Data?

A DNS TXT record to identify the printer.

var url: URL

The address of the printer.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Printer service discovery

class UIPrintServiceExtension

An extension that locates and sets up a printer without a configuration profile.

