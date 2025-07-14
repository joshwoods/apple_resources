

- Foundation
- NSValue
-  init(UIOffset:) 

Initializer

# init(UIOffset:)

Creates a new value object containing the specified UIKit offset structure.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(UIOffset insets: UIOffset)
```

``` source
init(uiOffset insets: UIOffset)
```

## Parameters 

`insets`  

The value for the new object.

## Return Value

A new value object that contains the offset information.

## See Also

### Related Documentation

struct UIOffset

A structure that specifies an amount to offset a position.

### Working with UIKit Geometry Values

init(UIEdgeInsets: UIEdgeInsets)

Creates a new value object containing the specified UIKit edge insets structure.

var uiEdgeInsetsValue: UIEdgeInsets

Returns the UIKit edge insets structure representation of the value.

var uiOffsetValue: UIOffset

Returns the UIKit offset structure representation of the value.

