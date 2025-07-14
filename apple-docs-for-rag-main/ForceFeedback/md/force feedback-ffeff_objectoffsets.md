

- Force Feedback
-  FFEFF_OBJECTOFFSETS 

Global Variable

# FFEFF_OBJECTOFFSETS

Mac Catalyst 13.0+macOS 10.2+

``` source
var FFEFF_OBJECTOFFSETS: UInt { get }
```

## Discussion

OBJECT IDS cannot be used to identify trigger buttons in FFEFFECT.dwTriggerButton, and output axes in FFEFFECT.rgdwAxes\[n\]. Please use object offsets (FFJOFS\_\* constants), the only supported method.

## See Also

### Constants

var E_PENDING: Int

var FF_DEGREES: Int32

var FF_DOWNLOADSKIPPED: HRESULT

var FF_EFFECTRESTARTED: HRESULT

var FF_FALSE: HRESULT

var FF_FFNOMINALMAX: Int32

var FF_INFINITE: UInt

var FF_OK: HRESULT

var FF_SECONDS: Int32

var FF_TRUNCATED: HRESULT

var FF_TRUNCATEDANDRESTARTED: HRESULT

var FFERR_DEVICEFULL: Int

var FFERR_DEVICEPAUSED: Int

var FFERR_DEVICERELEASED: Int

var FFERR_EFFECTPLAYING: Int

