

- AppKit
-  NSScrubberTextItemView 

Class

# NSScrubberTextItemView

A concrete view subclass for displaying text for an item in a scrubber.

macOS 10.12.2+

``` source
@MainActor
class NSScrubberTextItemView
```

## Overview

Provide the text you want to display in the scrubber item to the title property. If you want finer control over the appearance of the text, you can access the underlying text field using the textField property.

## Topics

### Providing text content

var title: String

The text displayed for the scrubber item.

var textField: NSTextField

The text field that the scrubber item uses to display its text.

## Relationships

### Inherits From

- NSScrubberItemView

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

class NSScrubberArrangedView

An abstract base class for the views whose layout is managed by a scrubber.

class NSScrubberImageItemView

A concrete view subclass for displaying images in a scrubber items.

class NSScrubberSelectionStyle

An abstract class that provides decorative accessory views for selected and highlighted items within a scrubber control.

class NSScrubberSelectionView

An abstract base class for specifying the appearance of a highlighted or selected item in a scrubber.

