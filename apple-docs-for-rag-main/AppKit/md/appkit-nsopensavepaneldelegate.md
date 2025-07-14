

- AppKit
-  NSOpenSavePanelDelegate 

Protocol

# NSOpenSavePanelDelegate

A set of methods for managing interactions with an open or save panel.

macOS

``` source
protocol NSOpenSavePanelDelegate : NSObjectProtocol
```

## Topics

### Responding to the User’s Selection

func panel(Any, userEnteredFilename: String, confirmed: Bool) -> String?

Tells the delegate that the user confirmed a filename choice by clicking Save in a Save panel.

### Responding to Panel Changes

func panelSelectionDidChange(Any?)

Tells the delegate that the user changed the selection in the specified Save panel.

func panel(Any, didChangeToDirectoryURL: URL?)

Tells the delegate that the user changed the selected directory to the directory located at the specified URL.

func panel(Any, willExpand: Bool)

Tells the delegate that the Save panel is about to expand or collapse because the user clicked the disclosure triangle that displays or hides the file browser.

### Validating the Panel Content

func panel(Any, shouldEnable: URL) -> Bool

Asks the delegate whether the specified URL should be enabled in the Open panel.

func panel(Any, validate: URL) throws

Asks the delegate to validate the URL for a file that the user selected.

### Instance Methods

func panel(Any, didSelect: UTType?)

`NSSavePanel`: Optional — Sent when the user changes the current type. `NSOpenPanel`: Not sent.

func panel(Any, displayNameFor: UTType) -> String?

`NSSavePanel`: Optional — Sent when the content type popup is displayed and the save panel needs the display name for a type. If `nil` is returned, the save panel will display type’s `localizedDescription`. `NSOpenPanel`: Not sent.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- NSPathCell

## See Also

### Open and Save Panels

class NSOpenPanel

A panel that prompts the user to select a file to open.

class NSSavePanel

A panel that prompts the user for information about where to save a file.

