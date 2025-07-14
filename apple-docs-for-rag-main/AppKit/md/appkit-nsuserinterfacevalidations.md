

- AppKit
-  NSUserInterfaceValidations 

Protocol

# NSUserInterfaceValidations

A protocol that a custom class can adopt to manage the enabled state of a UI element.

macOS

``` source
protocol NSUserInterfaceValidations
```

## Overview

The NSUserInterfaceValidations protocol works with the NSValidatedUserInterfaceItem protocol to allow the target of a user interface element such as a menu item or a toolbar item to decide whether or not the user interface element should be enabled.

Your custom classes should adopt this protocol if an instance may be the target of a user interface element and need to conditionally enable or disable the element based on the current state of the instance. For more details, read User Interface Validation.

## Topics

### Validating user interface items

func validateUserInterfaceItem(any NSValidatedUserInterfaceItem) -> Bool

Returns a Boolean value that indicates whether the sender should be enabled.

**Required**

## Relationships

### Conforming Types

- NSApplication
- NSButton
- NSColorPanel
- NSComboBox
- NSDocument
- NSDocumentController
- NSFontPanel
- NSForm
- NSMatrix
- NSOpenPanel
- NSOutlineView
- NSPanel
- NSPersistentDocument
- NSPopUpButton
- NSSavePanel
- NSSearchField
- NSSecureTextField
- NSSplitViewController
- NSStatusBarButton
- NSTableView
- NSTextField
- NSTextView
- NSTokenField
- NSWindow

## See Also

### UI Validation

protocol NSValidatedUserInterfaceItem

A protocol that a custom class can adopt to manage the automatic enablement of a UI control.

