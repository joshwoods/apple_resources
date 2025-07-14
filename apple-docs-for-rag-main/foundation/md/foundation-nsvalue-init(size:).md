

- Foundation
- NSValue
-  init(size:) 

Initializer

# init(size:)

Creates a new value object containing the specified Foundation size structure.

Mac Catalyst 13.0+macOS 10.0+

``` source
init(size: NSSize)
```

## Parameters 

`size`  

The value for the new object.

## Return Value

A new value object that contains the size information.

## See Also

### Related Documentation

typealias NSSize

A two-dimensional size.

### Working with Foundation Geometry Values

init(point: NSPoint)

Creates a new value object containing the specified Foundation point structure.

init(rect: NSRect)

Creates a new value object containing the specified Foundation rectangle structure.

var pointValue: NSPoint

The Foundation point structure representation of the value.

var sizeValue: NSSize

The Foundation size structure representation of the value.

var rectValue: NSRect

The Foundation rectangle structure representation of the value.

