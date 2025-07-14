

- Metal
- MTLVisibilityResultMode
-  MTLVisibilityResultMode.boolean 

Case

# MTLVisibilityResultMode.boolean

The result records whether any samples passed depth and stencil tests.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
case boolean
```

## Discussion

The GPU writes a 64-bit integer to the visibility result buffer that is nonzero if at least one fragment passed depth and stencil tests, and zero if no fragments passed the tests.

## See Also

### Constants

case disabled

The result doesn’t contain any data because visibility testing was disabled.

case counting

The result records how many samples passed depth and stencil tests.

