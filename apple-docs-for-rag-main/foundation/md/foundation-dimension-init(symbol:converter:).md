

- Foundation
- Dimension
-  init(symbol:converter:) 

Initializer

# init(symbol:converter:)

Initializes a dimensional unit with the symbol and unit converter you specify.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
init(
    symbol: String,
    converter: UnitConverter
)
```

## Parameters 

`symbol`  

The symbol used to represent the unit.

`converter`  

The unit converter used to represent the unit in terms of the dimension’s base unit.

## Return Value

A new dimensional unit with the specified symbol and unit converter.

## Discussion

This is the designated initializer.

