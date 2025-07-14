

- Metal
- MTLCommandQueue
-  label 

Instance Property

# label

An optional name that can help you identify the command queue.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var label: String? { get set }
```

**Required**

## Discussion

Set labels to help you quickly identify a GPU at runtime in the Metal debugging and profiling tools. See `Enhancing Frame Capture by Using Labels`.

## See Also

### Identifying the Command Queue

var device: any MTLDevice

The GPU device that creates the command queue.

**Required**

