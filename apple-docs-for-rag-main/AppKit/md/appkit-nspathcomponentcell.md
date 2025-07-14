

- AppKit
-  NSPathComponentCell 

Class

# NSPathComponentCell

A component of a path.

macOS 10.5+

``` source
@MainActor
class NSPathComponentCell
```

## Overview

An `NSPathCell` object manages a collection of `NSPathComponentCell` objects, in conjunction with an `NSPathControl` object, to represent a path.

## Topics

### Setting the Image

var image: NSImage?

The image displayed for this component cell.

### Setting the Path

var url: URL?

The portion of the path from the root through the component represented by the receiver.

## Relationships

### Inherits From

- NSTextFieldCell

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSCoding
- NSCopying
- NSObjectProtocol
- NSUserInterfaceItemIdentification
- Sendable

## See Also

### Cells

class NSPathCell

The user interface of a path control object.

protocol NSPathCellDelegate

A set of methods that enable the delegate of a path cell object to customize the Open panel or pop-up menu of a path whose style is set to NSPathControl.Style.popUp.

class NSPathControlItem

