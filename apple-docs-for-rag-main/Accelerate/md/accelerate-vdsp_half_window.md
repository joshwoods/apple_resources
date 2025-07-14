

- Accelerate
-  vDSP_HALF_WINDOW 

Global Variable

# vDSP_HALF_WINDOW

Specifies that the window should only contain the bottom half of the values (`0` to `(N+1)/2`).

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var vDSP_HALF_WINDOW: Int { get }
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

var vDSP_HANN_DENORM: Int

Specifies a denormalized Hann window.

var vDSP_HANN_NORM: Int

Specifies a normalized Hann window

