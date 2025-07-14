

- Accelerate
- vImage_YpCbCrPixelRange
-  YpMax 

Instance Property

# YpMax

The encoding for the maximum allowed Y’ value.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var YpMax: Int32
```

## Discussion

All values larger than this are clamped to this value.

## See Also

### Pixel Range Properties

var Yp_bias: Int32

The encoding for `Y' = 0.0` for this video format (varies by bit depth).

var CbCr_bias: Int32

The encoding for `{Cb, Cr} = 0.0` for this video format.

var YpRangeMax: Int32

The encoding for `Y' = 1.0` for this video format.

var CbCrRangeMax: Int32

The encoding for `{Cb, Cr} = 0.5` for this video format.

var YpMin: Int32

The encoding of the minimum allowed Y’ value.

var CbCrMax: Int32

The encoding of the maximum allowed `{Cb, Cr}` value.

var CbCrMin: Int32

The encoding of the minimum allowed `{Cb, Cr}` value.

