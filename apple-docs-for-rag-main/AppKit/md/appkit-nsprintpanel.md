

- AppKit
-  NSPrintPanel 

Class

# NSPrintPanel

The Print panel that queries the user for information about a print job.

macOS

``` source
@MainActor
class NSPrintPanel
```

## Overview

A Print panel may let the user select the range of pages to print and the number of copies before executing the Print command. Print panels can display a simplified interface when printing certain types of data. For example, the panel can display a list of print-setting presets, which lets the user enable print settings in groups as opposed to individually. Assigning an appropriate string to the jobStyleHint property activates the simplified interface and identifies which presets to display.

For design guidance, see Human Interface Guidelines.

## Topics

### Customizing the Panel

var jobStyleHint: NSPrintPanel.JobStyleHint?

The type of settings that the print panel displays.

struct JobStyleHint

Constants that specify job style hints for activating the simplified Print panel interface and setting the options to display.

var options: NSPrintPanel.Options

The current configuration options for the Print panel.

struct Options

Constants that specify options for configuring the contents of the main Print panel.

func defaultButtonTitle() -> String?

Returns the title of the Print panel’s default button.

func setDefaultButtonTitle(String?)

Sets the title of the Print panel’s default button.

var helpAnchor: NSHelpManager.AnchorName?

The HTML help anchor associated with the Print panel.

### Managing Accessory Views

func addAccessoryController(any NSViewController &amp; NSPrintPanelAccessorizing)

Adds a custom controller to the Print panel to manage an accessory view.

func removeAccessoryController(any NSViewController &amp; NSPrintPanelAccessorizing)

Removes the specified controller and accessory view from the Print panel.

protocol NSPrintPanelAccessorizing

A set of methods that a Print panel object can use to get information from a printing accessory controller.

var accessoryControllers: [NSViewController]

The array of controller objects that manage the Print panel’s accessory views.

### Running the Panel

func beginSheet(using: NSPrintInfo, on: NSWindow, completionHandler: ((NSPrintPanel.Result) -> Void)?)

func beginSheet(with: NSPrintInfo, modalFor: NSWindow, delegate: Any?, didEnd: Selector?, contextInfo: UnsafeMutableRawPointer?)

Displays a Print panel sheet and runs it modally for the specified window.

Deprecated

func runModal() -> Int

Displays the Print panel and begins the modal loop.

func runModal(with: NSPrintInfo) -> Int

Displays the Print panel and runs the modal loop using the specified printing information.

### Accessing the Printing Information

var printInfo: NSPrintInfo

The information associated with the running Print panel.

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

class NSPageLayout

A panel that queries the user for information such as paper type and orientation.

