

- SpriteKit
- SKRange
-  init(constantValue:) 

Initializer

# init(constantValue:)

Creates and initializes a new range object that specifies a constant value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
convenience init(constantValue value: CGFloat)
```

## Parameters 

`value`  

A constant.

## Return Value

A newly initialized range object whose minimum and maximum value are both equal to `value`.

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

init(lowerLimit: CGFloat, upperLimit: CGFloat)

Initializes a new range object.

