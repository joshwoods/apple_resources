

- AppKit
-  NSScrubberSelectionView 

Class

# NSScrubberSelectionView

An abstract base class for specifying the appearance of a highlighted or selected item in a scrubber.

macOS 10.12.2+

``` source
@MainActor
class NSScrubberSelectionView
```

## Overview

Create a subclass to customize the selection or highlight appearance of an item in your scrubber control. You need to return an instance of your subclass from the makeSelectionView() method on NSScrubberSelectionStyle.

## Relationships

### Inherits From

- NSScrubberArrangedView

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

class NSScrubberTextItemView

A concrete view subclass for displaying text for an item in a scrubber.

