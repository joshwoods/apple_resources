

- Accelerate
-  vclassifyf(\_:) 

Function

# vclassifyf(\_:)

For each vector element, returns the class of the argument (one of the FP\_ … constants defined in math.h).

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func vclassifyf(_: vFloat) -> vUInt32
```

## See Also

### Inquiry Functions (from vfp.h)

func vsignbitf(vFloat) -> vUInt32

For each vector element, returns a non-zero value if and only if the sign of `arg` is negative. This includes NaNs, infinities and zeros.

