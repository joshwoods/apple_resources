

- AppKit
-  NSScrubberSelectionStyle 

Class

# NSScrubberSelectionStyle

An abstract class that provides decorative accessory views for selected and highlighted items within a scrubber control.

macOS 10.12.2+

``` source
@MainActor
class NSScrubberSelectionStyle
```

## Overview

Choose a selection style (outlineOverlay or roundedBackground), or create a custom selection style by subclassing NSScrubberSelectionStyle and overriding makeSelectionView().

## Topics

### Using built-in styles

class var outlineOverlay: NSScrubberSelectionStyle

A built-in selection style that draws the outline of the scrubber item.

class var roundedBackground: NSScrubberSelectionStyle

A built-in selection style that draws a rounded rectangle as the background of the scrubber item.

### Creating a selection style

init()

Initializes a new scrubber selection style.

init(coder: NSCoder)

Initializes a scrubber selection style when included from a nib or Storyboard.

func makeSelectionView() -> NSScrubberSelectionView?

Provides an opportunity to create a customized scrubber selection style.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- Sendable

## See Also

### Scrubber items

class NSScrubberItemView

An item at a specific index position in the scrubber.

class NSScrubberArrangedView

An abstract base class for the views whose layout is managed by a scrubber.

class NSScrubberImageItemView

A concrete view subclass for displaying images in a scrubber items.

class NSScrubberSelectionView

An abstract base class for specifying the appearance of a highlighted or selected item in a scrubber.

class NSScrubberTextItemView

A concrete view subclass for displaying text for an item in a scrubber.

