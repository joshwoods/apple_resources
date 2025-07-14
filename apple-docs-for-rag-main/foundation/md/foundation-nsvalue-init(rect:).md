

- Foundation
- NSValue
-  init(rect:) 

Initializer

# init(rect:)

Creates a new value object containing the specified Foundation rectangle structure.

Mac Catalyst 13.0+macOS 10.0+

``` source
init(rect: NSRect)
```

## Parameters 

`rect`  

The value for the new object.

## Return Value

A new value object that contains the data in the `rect` structure.

## See Also

### Related Documentation

typealias NSRect

A rectangle.

### Working with Foundation Geometry Values

init(point: NSPoint)

Creates a new value object containing the specified Foundation point structure.

init(size: NSSize)

Creates a new value object containing the specified Foundation size structure.

var pointValue: NSPoint

The Foundation point structure representation of the value.

var sizeValue: NSSize

The Foundation size structure representation of the value.

var rectValue: NSRect

The Foundation rectangle structure representation of the value.

