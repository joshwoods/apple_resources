

- Quick Look UI
-  QLPreviewView 

Class

# QLPreviewView

A Quick Look preview of an item that you can embed into your view hierarchy.

macOS 10.6+

``` source
@MainActor
class QLPreviewView
```

## Topics

### Creating a Preview View

init!(frame: NSRect, style: QLPreviewViewStyle)

Creates a preview view with the provided frame and style.

init!(frame: NSRect)

Creates a preview view with the provided frame.

enum QLPreviewViewStyle

Styles for a Preview View.

### Displaying a Preview

var previewItem: (any QLPreviewItem)!

The item to preview.

func refreshPreviewItem()

Updates the preview to display the currently previewed item.

var displayState: Any!

The current display state of the previewItem.

var autostarts: Bool

A Boolean value that determines whether the preview starts automatically.

### Closing a Preview

var shouldCloseWithWindow: Bool

A Boolean value that determines whether the preview should close when its window closes.

func close()

Closes the view, releasing the current preview item.

## Relationships

### Inherits From

- NSView

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
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable

## See Also

### Previews

class QLPreviewPanel

A class that implements the Quick Look preview panel to display a preview of a list of items.

protocol QLPreviewItem

A protocol that defines a set of properties you implement to make a preview of your application’s content.

protocol QLPreviewPanelDataSource

A protocol that the Quick Look preview panel uses to access the contents of its data source object.

protocol QLPreviewPanelDelegate

A protocol for the delegate of the Quick Look preview panel.

typealias QLPreviewItemLoadingBlock

A type that defines a block used to load a Quick Look preview item.

Deprecated

