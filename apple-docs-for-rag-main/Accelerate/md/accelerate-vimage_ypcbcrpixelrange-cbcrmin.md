

- Accelerate
- vImage_YpCbCrPixelRange
-  CbCrMin 

Instance Property

# CbCrMin

The encoding of the minimum allowed `{Cb, Cr}` value.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var CbCrMin: Int32
```

## Discussion

All chroma values less than this value will be clamped to this value.

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

var YpMax: Int32

The encoding for the maximum allowed Y’ value.

var YpMin: Int32

The encoding of the minimum allowed Y’ value.

var CbCrMax: Int32

The encoding of the maximum allowed `{Cb, Cr}` value.

