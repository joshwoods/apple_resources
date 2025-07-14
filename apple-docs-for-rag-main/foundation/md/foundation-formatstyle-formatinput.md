

- Foundation
- FormatStyle
-  FormatInput 

Associated Type

# FormatInput

The type this format style accepts as input.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
associatedtype FormatInput
```

**Required**

## Discussion

Swift type inference uses this value to determine which static accessors are available at a given call point. For example, when you format an Int32, you can use the static number property that provies a `IntegerFormatStyle`, as seen in the following example. This works because the style’s input type `IntegerFormatStyle/FormatInput` is a BinaryInteger generically constrained to the Int32 type.

```
let perihelionDistanceToSunInKm: Int32 = 147098291
perihelionDistanceToSunInKm.formatted(.number
    .notation(.scientific)) // "1.470983E8"
```

## See Also

### Declaring input and output types

associatedtype FormatOutput

The type this format style produces as output.

**Required**

