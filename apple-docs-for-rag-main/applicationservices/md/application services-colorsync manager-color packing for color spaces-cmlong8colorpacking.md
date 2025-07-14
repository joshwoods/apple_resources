

- Application Services
- ColorSync Manager
- Color Packing for Color Spaces
-  cmLong8ColorPacking 

Global Variable

# cmLong8ColorPacking

macOS 10.0+

``` source
var cmLong8ColorPacking: Int { get }
```

## Discussion

The color values for three or four 8-bit color channels are stored consecutively in a 32-bit long. For three channels, this constant is combined with either `cmAlphaFirstPacking` or `cmAlphaLastPacking` to indicate whether the unused eight bits are located at the beginning or end.

