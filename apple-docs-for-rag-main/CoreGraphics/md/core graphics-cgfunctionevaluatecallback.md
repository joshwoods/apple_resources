

- Core Graphics
-  CGFunctionEvaluateCallback 

Type Alias

# CGFunctionEvaluateCallback

Performs custom operations on the supplied input data to produce output data.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CGFunctionEvaluateCallback = (UnsafeMutableRawPointer?, UnsafePointer, UnsafeMutablePointer) -> Void
```

## Parameters 

`info`  

The `info` parameter passed to init(info:domainDimension:domain:rangeDimension:range:callbacks:).

`inData`  

An array of floats. The size of the array is that specified by the `domainDimension` parameter passed to the init(info:domainDimension:domain:rangeDimension:range:callbacks:) function.

`outData`  

An array of floats. The size of the array is that specified by the `rangeDimension` parameter passed to the init(info:domainDimension:domain:rangeDimension:range:callbacks:) function.

## Discussion

The callback you write is responsible for implementing thecalculation of output values from the supplied input values. Forexample, if you want to implement a simple “squaring” functionof one input argument to one output argument, your evaluation functionmight be:

```
void evaluateSquare(void *info, const float *inData, float *outData)
{
    outData[0] = inData[0] * inData[0];
}
```

## See Also

### Callbacks

struct CGFunctionCallbacks

A structure that contains callbacks needed by a `CGFunctionRef` object.

typealias CGFunctionReleaseInfoCallback

Performs custom clean-up tasks when Core Graphics deallocates a `CGFunctionRef` object.

