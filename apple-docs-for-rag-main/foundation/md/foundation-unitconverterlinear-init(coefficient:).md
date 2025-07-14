

- Foundation
- UnitConverterLinear
-  init(coefficient:) 

Initializer

# init(coefficient:)

Initializes the unit converter with the coefficient you specify.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
convenience init(coefficient: Double)
```

## Parameters 

`coefficient`  

The coefficient used in the linear unit conversion calculation.

## Return Value

A unit converter initialized with the specified coefficient.

## Discussion

Calling this initializer is equivalent to calling init(coefficient:constant:), passing `0` for the `constant` parameter.

## See Also

### Creating Unit Converters

init(coefficient: Double, constant: Double)

Creates a unit converter with the coefficient and constant you specify.

