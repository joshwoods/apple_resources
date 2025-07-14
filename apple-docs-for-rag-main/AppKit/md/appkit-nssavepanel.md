

- AppKit
-  NSSavePanel 

Class

# NSSavePanel

A panel that prompts the user for information about where to save a file.

macOS

``` source
@MainActor
class NSSavePanel
```

## Overview

The Save panel provides an interface for specifying the location to save a file and the name of that file. You present this panel when the user attempts to save a new document, or when the user saves a copy of an existing document to a new location. The panel includes UI for browsing the file system, selecting a directory, and specifying the new name for the file. You can also add custom UI for your app using an accessory view.

An NSSavePanel object reports user interactions to its associated delegate object, which must adopt the NSOpenSavePanelDelegate protocol. Use your delegate object to validate the user’s selection and respond to user interactions with the panel.

In macOS 10.15, the system always displays the Save dialog in a separate process, regardless of whether the app is sandboxed. When the user saves the document, macOS adds the saved file to the app’s sandbox (if necessary) so that the app can write to the file. Prior to macOS 10.15, the system used a separate process only for sandboxed apps.

## Topics

### Responding to User Interactions

var delegate: (any NSOpenSavePanelDelegate)?

A custom object you use to manage interactions with an open or save panel.

protocol NSOpenSavePanelDelegate

A set of methods for managing interactions with an open or save panel.

### Showing the Panel

func beginSheetModal(for: NSWindow, completionHandler: (NSApplication.ModalResponse) -> Void)

Presents the panel as a sheet modal to the specified window.

func begin(completionHandler: (NSApplication.ModalResponse) -> Void)

Presents the panel as a modeless window.

func runModal() -> NSApplication.ModalResponse

Displays the panel and begins its event loop with the current working (or last-selected) directory as the default starting point.

func validateVisibleColumns()

Validates and reloads the browser columns visible in the panel.

### Getting the Selected Item

var url: URL?

A URL that contains the fully specified location of the targeted file.

### Configuring the Panel’s Appearance

var title: String!

The title of the panel.

var prompt: String!

The text to display in the default button.

var message: String!

The message text displayed in the panel.

var nameFieldLabel: String!

The label text displayed in front of the filename text field.

var nameFieldStringValue: String

The user-editable filename currently shown in the name field.

var directoryURL: URL?

The current directory shown in the panel.

var accessoryView: NSView?

The custom accessory view for the current app.

var showsTagField: Bool

A Boolean value that indicates whether the panel displays the Tags field.

var tagNames: [String]?

The tag names that you want to include on a saved file.

### Configuring the Panel’s Behavior

var canCreateDirectories: Bool

A Boolean value that indicates whether the panel displays UI for creating directories.

var canSelectHiddenExtension: Bool

A Boolean value that indicates whether the panel displays UI for hiding or showing filename extensions.

var showsHiddenFiles: Bool

A Boolean value that indicates whether the panel displays files that are normally hidden from the user.

var isExtensionHidden: Bool

A Boolean value that indicates whether to display filename extensions.

var isExpanded: Bool

A Boolean value that indicates whether whether the panel is expanded.

Button tags

Button tags that refer to items on the panel.

### Configuring the File Types

var allowedContentTypes: [UTType]

An array of types that specify the files types to which you can save.

var allowsOtherFileTypes: Bool

A Boolean value that indicates whether the panel allows the user to save files with a filename extension that’s not in the list of allowed types.

var treatsFilePackagesAsDirectories: Bool

A Boolean value that indicates whether the panel displays file packages as directories.

### Handling Actions

func ok(Any?)

The action method that the panel calls when the user clicks the OK button.

func cancel(Any?)

The action method that the panel calls when the user clicks the Cancel button.

### Deprecated

Avoid using deprecated classes and protocols in your apps.

Deprecated Symbols

Review unsupported symbols and their replacements.

### Instance Properties

var identifier: NSUserInterfaceItemIdentifier?

var currentContentType: UTType?

`NSSavePanel`:The current type. If set to `nil`, resets to the first allowed content type. Returns `nil` if `allowedContentTypes` is empty. `NSOpenPanel`: Not used.

var showsContentTypes: Bool

`NSSavePanel`: Whether or not to show a control for selecting the type of the saved file. The control shows the types in `allowedContentTypes`. Default is `NO`.

## Relationships

### Inherits From

- NSPanel

### Inherited By

- NSOpenPanel

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSMenuItemValidation
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- NSUserInterfaceValidations
- Sendable

## See Also

### Open and Save Panels

class NSOpenPanel

A panel that prompts the user to select a file to open.

protocol NSOpenSavePanelDelegate

A set of methods for managing interactions with an open or save panel.

