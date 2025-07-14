

- ML Compute
- MLCSplitLayer
-  splitCount Deprecated

Instance Property

# splitCount

The number of splits.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
var splitCount: Int { get }
```

## Discussion

The layer splits the tensor into equally sized chunks, however the last chunk may be smaller in size.

## See Also

### Inspecting Split Layers

var dimension: Int

The dimension or axis along which to split the tensor.

Deprecated

var splitSectionLengths: [Int]?

An array that contains the lengths of each split section.

Deprecated

