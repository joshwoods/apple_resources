

- AppKit
-  NSScrubberArrangedView 

Class

# NSScrubberArrangedView

An abstract base class for the views whose layout is managed by a scrubber.

macOS 10.12.2+

``` source
@MainActor
class NSScrubberArrangedView
```

## Topics

### Managing selection and highlighting

var isHighlighted: Bool

A Boolean value that specifies whether the view is currently highlighted.

var isSelected: Bool

A Boolean value that specifies whether the current view is selected.

### Controlling the layout

func apply(NSScrubberLayoutAttributes)

Updates the layout of the arranged view to respect the provided layout attributes.

## Relationships

### Inherits From

- NSView

### Inherited By

- NSScrubberItemView
- NSScrubberSelectionView

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

### Scrubber items

class NSScrubberItemView

An item at a specific index position in the scrubber.

class NSScrubberImageItemView

A concrete view subclass for displaying images in a scrubber items.

class NSScrubberSelectionStyle

An abstract class that provides decorative accessory views for selected and highlighted items within a scrubber control.

class NSScrubberSelectionView

An abstract base class for specifying the appearance of a highlighted or selected item in a scrubber.

class NSScrubberTextItemView

A concrete view subclass for displaying text for an item in a scrubber.

