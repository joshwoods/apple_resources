

- Accelerate
-  vDSP_HANN_DENORM 

Global Variable

# vDSP_HANN_DENORM

Specifies a denormalized Hann window.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var vDSP_HANN_DENORM: Int { get }
```

## See Also

### Vector generation with window functions

Reducing spectral leakage with windowing

Multiply signal data by window sequence values when performing transforms with noninteger period signals.

static func window&lt;T>(ofType: T.Type, usingSequence: vDSP.WindowSequence, count: Int, isHalfWindow: Bool) -> [T]

Returns an array that contains the specified window.

static func formWindow&lt;V>(usingSequence: vDSP.WindowSequence, result: inout V, isHalfWindow: Bool)

Populates a double-precision vector with a specified window.

static func formWindow&lt;V>(usingSequence: vDSP.WindowSequence, result: inout V, isHalfWindow: Bool)

Populates a single-precision vector with a specified window.

enum WindowSequence

Constants that specify window sequence functions.

var vDSP_HALF_WINDOW: Int

Specifies that the window should only contain the bottom half of the values (`0` to `(N+1)/2`).

var vDSP_HANN_NORM: Int

Specifies a normalized Hann window

