

- SpriteKit
- SKRange
-  init(upperLimit:) 

Initializer

# init(upperLimit:)

Creates and initializes a new range object that specifies only a maximum value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
convenience init(upperLimit upper: CGFloat)
```

## Parameters 

`upper`  

The maximum value for the range.

## Return Value

A newly initialized range object whose minimum value is `-Inf` and whose maximum value is `upper`.

## See Also

### Creating a Range Object

convenience init(value: CGFloat, variance: CGFloat)

Creates and initializes a new range object using a value and a maximum distance from that value.

class func withNoLimits() -> Self

Creates and initializes a new range object that encompasses all possible values.

convenience init(lowerLimit: CGFloat)

Creates and initializes a new range object that specifies only a minimum value.

convenience init(constantValue: CGFloat)

Creates and initializes a new range object that specifies a constant value.

init(lowerLimit: CGFloat, upperLimit: CGFloat)

Initializes a new range object.

