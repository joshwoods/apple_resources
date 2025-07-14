

- Metal
- MTLVertexBufferLayoutDescriptor
-  stride 

Instance Property

# stride

The number of bytes between the first byte of two consecutive vertices in a buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var stride: Int { get set }
```

## Discussion

Check the Metal feature set tables (PDF) for potential alignment restrictions for `stride`.

## See Also

### Organizing the Vertex Buffer Layout

var stepFunction: MTLVertexStepFunction

The circumstances under which the vertex and its attributes are presented to the vertex function.

var stepRate: Int

The interval at which the vertex and its attributes are presented to the vertex function.

