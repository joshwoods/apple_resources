

- Metal
- MTLVertexBufferLayoutDescriptor
-  stepRate 

Instance Property

# stepRate

The interval at which the vertex and its attributes are presented to the vertex function.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var stepRate: Int { get set }
```

## Discussion

The default value is `1`. The `stepRate` value, in conjunction with the stepFunction property, determines how often the function fetches new attribute data. The `stepRate` property is generally used when `stepFunction` is MTLVertexStepFunction.perInstance. If `stepRate` is equal to `1`, new attribute data is fetched for every instance; if `stepRate` is equal to `2`, new attribute data is fetched for every two instances, and so forth.

## See Also

### Organizing the Vertex Buffer Layout

var stepFunction: MTLVertexStepFunction

The circumstances under which the vertex and its attributes are presented to the vertex function.

var stride: Int

The number of bytes between the first byte of two consecutive vertices in a buffer.

