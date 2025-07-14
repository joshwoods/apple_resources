

- UIKit
-  UIPrintServiceExtension 

Class

# UIPrintServiceExtension

An extension that locates and sets up a printer without a configuration profile.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+visionOS 1.0+

``` source
@MainActor
class UIPrintServiceExtension
```

## Overview

Support cloud printing by creating an extension instead of requiring users to install a managed configuration profile to set up an AirPrint printer. Create an extension by subclassing `UIPrintServiceExtension`. By creating your own extension, you can expose a cloud printer destination to a UIPrinterPickerController. The extension matches printer destinations that fulfill the specified print-job attributes.

Create an instance of `UIPrinterDestination` to describe a printer to the system. The extension can then search for the printer, or set of printers, using printerDestinations(for:). This method matches the requirements of a UIPrintInfo object and returns an array of UIPrinterDestination.

## Topics

### Locating a printer

func printerDestinations(for: UIPrintInfo) -> [UIPrinterDestination]

Searches for a printer destination that matches the print-job attributes.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Related Documentation

App extensions

Extend your app’s basic functionality to other parts of the system.

### Printer service discovery

class UIPrinterDestination

A description of a single printer.

