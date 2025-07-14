

- SpriteKit
- SKRange
-  init(lowerLimit:upperLimit:) 

Initializer

# init(lowerLimit:upperLimit:)

Initializes a new range object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init(
    lowerLimit lower: CGFloat,
    upperLimit upper: CGFloat
)
```

## Parameters 

`lower`  

The minimum value for the range.

`upper`  

The maximum value for the range.

## Return Value

A newly initialized range object.

## See Also

### Creating a Range Object

convenience init(value: CGFloat, variance: CGFloat)

Creates and initializes a new range object using a value and a maximum distance from that value.

class func withNoLimits() -> Self

Creates and initializes a new range object that encompasses all possible values.

convenience init(lowerLimit: CGFloat)

Creates and initializes a new range object that specifies only a minimum value.

convenience init(upperLimit: CGFloat)

Creates and initializes a new range object that specifies only a maximum value.

convenience init(constantValue: CGFloat)

Creates and initializes a new range object that specifies a constant value.

