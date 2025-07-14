

- GSS
-  GSS_C_CALLING_ERROR_MASK 

Global Variable

# GSS_C_CALLING_ERROR_MASK

A mask with a width that matches the calling error field.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.14+visionOS 1.0+

``` source
var GSS_C_CALLING_ERROR_MASK: UInt { get }
```

## Discussion

Shift the mask to the left by GSS_C_CALLING_ERROR_OFFSET to put it in the correct position within the major status code to match the calling error field. The GSS_CALLING_ERROR macro does this for you, before bitwise `AND`ing with its input.

## See Also

### Masks and Offsets

var GSS_C_CALLING_ERROR_OFFSET: Int32

The offset of the calling error field within the major status code.

var GSS_C_ROUTINE_ERROR_MASK: UInt

A mask with a width that matches the routine error field.

var GSS_C_ROUTINE_ERROR_OFFSET: Int32

The offset of the routine error field within the major status code.

var GSS_C_SUPPLEMENTARY_MASK: UInt

A mask with a width that matches the supplementary information field.

var GSS_C_SUPPLEMENTARY_OFFSET: Int32

The offset of the supplementary information field within the major status code.

