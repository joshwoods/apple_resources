

- AppKit
-  NSPDFPanel 

Class

# NSPDFPanel

A Save or Export as PDF panel that’s consistent with the macOS user interface.

macOS 10.9+

``` source
@MainActor
class NSPDFPanel
```

## Overview

A PDF panel has a variety of built-in customization controls, such as page orientation, paper size, and tags. It also supports the use of a custom accessory view controller that allows an app to specify how a PDF file should be created.

## Topics

### Managing the Contents of a PDF Panel

var accessoryController: NSViewController?

A view controller for the accessory view that the panel can present.

var options: NSPDFPanel.Options

A set of configuration options that determine the accessory views the PDF panel should display.

var defaultFileName: String

The initial value for the user-editable filename shown in the name field of the PDF panel.

### Displaying a PDF Panel

func beginSheet(with: NSPDFInfo, modalFor: NSWindow?, completionHandler: (Int) -> Void)

Presents a document-modal PDF panel.

### Constants

struct Options

Constants used to configure the contents of a PDF panel.

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

### Print and PDF Panels

protocol NSPrintPanelAccessorizing

A set of methods that a Print panel object can use to get information from a printing accessory controller.

