

- Metal
- MTLBlendOperation
-  MTLBlendOperation.subtract 

Case

# MTLBlendOperation.subtract

Subtract a portion of the destination pixel values from a portion of the source.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
case subtract
```

## Discussion

`RGB = Source.rgb * SBF - Dest.rgb * DBF`

`A = Source.a * SBF - Dest.a * DBF`

## See Also

### Constants

case add

Add portions of both source and destination pixel values.

case reverseSubtract

Subtract a portion of the source values from a portion of the destination pixel values.

case min

Minimum of the source and destination pixel values.

case max

Maximum of the source and destination pixel values.

