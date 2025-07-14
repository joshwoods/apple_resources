

- Metal
- MTLCommandEncoder
-  label 

Instance Property

# label

A string that labels the command encoder.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var label: String? { get set }
```

**Required**

## Discussion

Object and command labels are useful identifiers at runtime or when profiling and debugging your app using any Metal tool. See `Enhancing Frame Capture by Using Labels`.

## See Also

### Identifying the Command Encoder

var device: any MTLDevice

The Metal device from which the command encoder was created.

**Required**

