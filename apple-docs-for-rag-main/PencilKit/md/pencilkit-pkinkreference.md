

- PencilKit
-  PKInkReference 

Class

# PKInkReference

Provides a description of the creation and rendering of marks on a canvas.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
class PKInkReference
```

## Topics

### Creating an ink

init(inkType: __PKInkType, color: UIColor)

Create a new ink, specifying its type, color.

### Getting the ink attributes

var color: UIColor

The base color for this ink.

var inkType: __PKInkType

The type of ink, such as pen or pencil, as defined in the PKInkType enumeration.

### Supporting backward compatibility

var requiredContentVersion: PKContentVersion

The version of PencilKit necessary to use the ink.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

