

- Metal
- MTLBlendOperation
-  MTLBlendOperation.reverseSubtract 

Case

# MTLBlendOperation.reverseSubtract

Subtract a portion of the source values from a portion of the destination pixel values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
case reverseSubtract
```

## Discussion

`RGB = Dest.rgb * DBF - Source.rgb * SBF`

`A = Dest.a * DBF - Source.a * SBF`

## See Also

### Constants

case add

Add portions of both source and destination pixel values.

case subtract

Subtract a portion of the destination pixel values from a portion of the source.

case min

Minimum of the source and destination pixel values.

case max

Maximum of the source and destination pixel values.

