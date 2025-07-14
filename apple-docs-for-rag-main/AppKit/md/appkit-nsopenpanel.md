

- AppKit
-  NSOpenPanel 

Class

# NSOpenPanel

A panel that prompts the user to select a file to open.

macOS

``` source
@MainActor
class NSOpenPanel
```

## Overview

Apps use the Open panel as a convenient way to query the user for the name of a file to open. In macOS 10.15 and later, the system always draws Open panels in a separate process, regardless of whether the app is sandboxed. When the user chooses a file to open, macOS adds that file to the app’s sandbox. Prior to macOS 10.15, the system drew the panels in a separate process only for sandboxed apps.

## Topics

### Configuring the Open Panel

var canChooseFiles: Bool

A Boolean that indicates whether the user can choose files in the panel.

var canChooseDirectories: Bool

A Boolean that indicates whether the user can choose directories in the panel.

var resolvesAliases: Bool

A Boolean that indicates whether the panel resolves aliases.

var allowsMultipleSelection: Bool

A Boolean that indicates whether the user may select multiple files and directories.

var isAccessoryViewDisclosed: Bool

A Boolean value that indicates whether the panel’s accessory view is visible.

### Accessing User Selection

var urls: [URL]

An array of URLs, each of which contains the fully specified location of a selected file or directory.

### Supporting iCloud Documents

var canDownloadUbiquitousContents: Bool

A Boolean value that indicates how the panel responds to iCloud documents that aren’t fully downloaded locally.

var canResolveUbiquitousConflicts: Bool

A Boolean value that indicates how the panel responds to iCloud documents that have conflicting versions.

### Deprecated

Avoid using deprecated classes and protocols in your apps.

Deprecated Symbols

Review symbols that are no longer supported, and find the replacements to use instead.

## Relationships

### Inherits From

- NSSavePanel

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

class NSSavePanel

A panel that prompts the user for information about where to save a file.

protocol NSOpenSavePanelDelegate

A set of methods for managing interactions with an open or save panel.

