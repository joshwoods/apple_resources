

- Accelerate
- vImage_YpCbCrPixelRange
-  CbCrRangeMax 

Instance Property

# CbCrRangeMax

The encoding for `{Cb, Cr} = 0.5` for this video format.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var CbCrRangeMax: Int32
```

## Discussion

This is usually near the high end of the encodable range (e.g. `0xf0`), if not the maximum encodable value (e.g. `0xff`).

## See Also

### Pixel Range Properties

var Yp_bias: Int32

The encoding for `Y' = 0.0` for this video format (varies by bit depth).

var CbCr_bias: Int32

The encoding for `{Cb, Cr} = 0.0` for this video format.

var YpRangeMax: Int32

The encoding for `Y' = 1.0` for this video format.

var YpMax: Int32

The encoding for the maximum allowed Y’ value.

var YpMin: Int32

The encoding of the minimum allowed Y’ value.

var CbCrMax: Int32

The encoding of the maximum allowed `{Cb, Cr}` value.

var CbCrMin: Int32

The encoding of the minimum allowed `{Cb, Cr}` value.

