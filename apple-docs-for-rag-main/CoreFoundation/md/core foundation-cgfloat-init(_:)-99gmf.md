

- Core Foundation
- CGFloat
-  init(\_:) 

Initializer

# init(\_:)

Creates a new value, rounded to the closest possible representation.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.10+tvOS 9.0+visionOSwatchOS 2.0+SwiftDeprecated

``` source
init(_ number: NSNumber)
```

## Parameters 

`number`  

The number to convert to a floating-point value.

## Discussion

If two representable values are equally close, the result is the value with more trailing zeros in its significand bit pattern.

