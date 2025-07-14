

- ML Compute
- MLCTensorData
-  length Deprecated

Instance Property

# length

The number of bytes you choose to hold for this tensor data instance.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
var length: Int { get }
```

## Discussion

Important

This value must not exceed length of `bytes`.

## See Also

### Inspecting Tensor Data

var bytes: UnsafeMutableRawPointer

A buffer that conains data.

Deprecated

