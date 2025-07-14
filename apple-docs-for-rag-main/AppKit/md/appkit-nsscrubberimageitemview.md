

- AppKit
-  NSScrubberImageItemView 

Class

# NSScrubberImageItemView

A concrete view subclass for displaying images in a scrubber items.

macOS 10.12.2+

``` source
@MainActor
class NSScrubberImageItemView
```

## Overview

Provide the image you want to display in the scrubber item to the image property. If you want finer control over the appearance of the image, you can access the underlying image view using the imageView property.

The image is scaled proportionally to fit the view’s frame. Use the imageAlignment property to determine how the scaled image is cropped within that frame.

## Topics

### Providing image content

var image: NSImage

The image displayed by the scrubber item.

var imageView: NSImageView

The image view that the scrubber item uses to display its image.

### Configuring the appearance

var imageAlignment: NSImageAlignment

The alignment of the image within the scrubber item.

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

class NSScrubberSelectionStyle

An abstract class that provides decorative accessory views for selected and highlighted items within a scrubber control.

class NSScrubberSelectionView

An abstract base class for specifying the appearance of a highlighted or selected item in a scrubber.

class NSScrubberTextItemView

A concrete view subclass for displaying text for an item in a scrubber.

