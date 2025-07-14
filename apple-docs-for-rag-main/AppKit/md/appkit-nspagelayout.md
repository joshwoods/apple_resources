

- AppKit
-  NSPageLayout 

Class

# NSPageLayout

A panel that queries the user for information such as paper type and orientation.

macOS

``` source
@MainActor
class NSPageLayout
```

## Overview

A page layout panel is typically displayed in response to the user selecting the Page Setup menu item. You obtain an instance with the pageLayout class method. The pane can then be run as a sheet using beginSheet(with:modalFor:delegate:didEnd:contextInfo:) or modally using runModal() or runModal(with:).

For design guidance, see Human Interface Guidelines.

## Topics

### Running the page setup dialog

func beginSheet(using: NSPrintInfo, on: NSWindow, completionHandler: ((NSPageLayout.Result) -> Void)?)

func beginSheet(with: NSPrintInfo, modalFor: NSWindow, delegate: Any?, didEnd: Selector?, contextInfo: UnsafeMutableRawPointer?)

Presents a page setup sheet for the specified print info object, document-modal relative to the specified window.

Deprecated

func runModal() -> Int

Displays the page layout panel and begins the modal loop using the shared print info object.

func runModal(with: NSPrintInfo) -> Int

Displays the page layout panel and begins the modal loop using the specified print info object.

### Customizing the page setup dialog

func addAccessoryController(NSViewController)

Adds the specified controller of an accessory view to be presented in the page setup panel.

func removeAccessoryController(NSViewController)

Removes the specified controller of an accessory view.

var accessoryControllers: [NSViewController]

An array of accessory view controllers belonging to the page layout panel.

### Accessing the printing information

var printInfo: NSPrintInfo?

The printing information object used when the page layout panel is run.

class NSPrintInfo

An object that stores information that’s used to generate printed output.

enum Result

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

### Print Panels

class NSPrintPanel

The Print panel that queries the user for information about a print job.

