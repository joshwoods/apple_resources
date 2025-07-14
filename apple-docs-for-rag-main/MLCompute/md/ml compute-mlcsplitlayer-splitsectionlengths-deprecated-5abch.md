

- ML Compute
- MLCSplitLayer
-  splitSectionLengths Deprecated

Instance Property

# splitSectionLengths

An array that contains the lengths of each split section.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0Deprecated

``` source
var splitSectionLengths: [Int]? { get }
```

Deprecated

Use Metal Performance Shaders Graph or BNNS instead.

## Discussion

The layer splits the tensor into chunks along dimensions with sizes given in `splitSectionLengths`.

## See Also

### Inspecting Split Layers

var dimension: Int

The dimension or axis along which to split the tensor.

Deprecated

var splitCount: Int

The number of splits.

Deprecated

