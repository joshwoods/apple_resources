

- PencilKit
-  PKToolPickerItem 

Class

# PKToolPickerItem

The base class for an item in the tool picker.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
class PKToolPickerItem
```

## Topics

### Identifying the item

var identifier: String

A string that identifies the item in the tool picker.

## Relationships

### Inherits From

- NSObject

### Inherited By

- PKToolPickerCustomItem
- PKToolPickerEraserItem
- PKToolPickerInkingItem
- PKToolPickerLassoItem
- PKToolPickerRulerItem
- PKToolPickerScribbleItem

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Creating a tool picker

init()

Creates a new tool picker with a default set of tools.

init(toolItems: [PKToolPickerItem])

Creates a new tool picker with the tools you specify.

class PKToolPickerInkingItem

An item that represents an inking tool in the tool picker.

class PKToolPickerEraserItem

An item that represents an eraser tool in the tool picker.

class PKToolPickerLassoItem

An item that represents a lasso tool in the tool picker.

class PKToolPickerRulerItem

An item that represents a ruler tool in the tool picker.

class PKToolPickerScribbleItem

An item that represents a Scribble tool in the tool picker.

class PKToolPickerCustomItem

An item that represents a custom tool in the tool picker.

