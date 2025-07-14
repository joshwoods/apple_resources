

- Quick Look UI
-  QLPreviewPanel 

Class

# QLPreviewPanel

A class that implements the Quick Look preview panel to display a preview of a list of items.

macOS 10.6+

``` source
@MainActor
class QLPreviewPanel
```

## Overview

Every application has a single shared instance of QLPreviewPanel accessible through shared(). The preview panel follows the responder chain and adapts to the first responder willing to control it. A preview panel controller provides the content through methods defined in the QLPreviewPanelDataSource protocol.

You can’t subclass QLPreviewPanel; you can, however, customize its behavior using a delegate. See the QLPreviewPanelDelegate protocol for the methods to customize a preview panel’s behavior.

## Topics

### Accessing the Shared Panel

class func shared() -> QLPreviewPanel!

Returns the shared Quick Look preview panel instance.

class func sharedPreviewPanelExists() -> Bool

Returns a Boolean value that indicates whether the system has created a shared Quick Look preview panel.

### Accessing the Preview Panel Controller

var currentController: Any!

The current first responder accepting to control the preview panel.

func updateController()

Asks the preview panel to update its current controller.

### Managing the Preview Items

var dataSource: (any QLPreviewPanelDataSource)!

The preview panel data source.

func reloadData()

Asks the preview panel to reload its data from its data source.

func refreshCurrentPreviewItem()

Asks the preview panel to recompute the preview of the current preview item.

var currentPreviewItemIndex: Int

The index of the current preview item.

var currentPreviewItem: (any QLPreviewItem)!

The currently previewed item.

var displayState: Any!

The preview panel’s display state.

### The Panel’s Delegate

var delegate: AnyObject!

The delegate object that controls the preview panel’s behavior.

### Managing Full Screen Mode

func enterFullScreenMode(NSScreen!, withOptions: [AnyHashable : Any]!) -> Bool

Instructs the panel to enter full screen mode.

func exitFullScreenMode(options: [AnyHashable : Any]!)

Instructs the panel to exit full screen mode.

var isInFullScreenMode: Bool

The property that indicates whether the panel is in full screen mode.

## Relationships

### Inherits From

- NSPanel

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

## See Also

### Previews

class QLPreviewView

A Quick Look preview of an item that you can embed into your view hierarchy.

protocol QLPreviewItem

A protocol that defines a set of properties you implement to make a preview of your application’s content.

protocol QLPreviewPanelDataSource

A protocol that the Quick Look preview panel uses to access the contents of its data source object.

protocol QLPreviewPanelDelegate

A protocol for the delegate of the Quick Look preview panel.

typealias QLPreviewItemLoadingBlock

A type that defines a block used to load a Quick Look preview item.

Deprecated

