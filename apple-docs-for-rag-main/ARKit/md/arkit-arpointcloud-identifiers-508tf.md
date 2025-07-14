

- ARKit
- ARPointCloud
-  identifiers 

Instance Property

# identifiers

A list of unique identifiers corresponding to detected feature points.

iOS 11.0+iPadOS 11.0+

``` source
@nonobjc
var identifiers: [UInt64] { get }
```

## Discussion

Each identifier in this list corresponds to the point vector at the same index in the points array.

## See Also

### Identifying Feature Points

var points: [simd_float3]

The list of detected points.

