

- SpriteKit
- SKRange
-  init(value:variance:) 

Initializer

# init(value:variance:)

Creates and initializes a new range object using a value and a maximum distance from that value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
convenience init(
    value: CGFloat,
    variance: CGFloat
)
```

## Parameters 

`value`  

The midpoint for the range.

`variance`  

The maximum amount that a value may differ from the midpoint.

## Return Value

A newly initialized range object whose minimum value is `value-variance` and whose maximum value is `value+variance`.

## See Also

### Creating a Range Object

class func withNoLimits() -> Self

Creates and initializes a new range object that encompasses all possible values.

convenience init(lowerLimit: CGFloat)

Creates and initializes a new range object that specifies only a minimum value.

convenience init(upperLimit: CGFloat)

Creates and initializes a new range object that specifies only a maximum value.

convenience init(constantValue: CGFloat)

Creates and initializes a new range object that specifies a constant value.

init(lowerLimit: CGFloat, upperLimit: CGFloat)

Initializes a new range object.

