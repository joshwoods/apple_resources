

- Metal
- MTLCommandEncoder
-  endEncoding() 

Instance Method

# endEncoding()

Declares that all command generation from the encoder is completed.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func endEncoding()
```

**Required**

## Discussion

After `endEncoding` is called, the command encoder has no further use. You cannot encode any other commands with this encoder.

## See Also

### Related Documentation

Metal Shading Language Guide

Metal Programming Guide

