

- Metal
- MTLArgumentEncoder
-  label 

Instance Property

# label

A string that identifies the argument buffer.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var label: String? { get set }
```

**Required**

## Discussion

Object and command labels are useful identifiers at runtime or when profiling and debugging your app using any Metal tool. See `Enhancing Frame Capture by Using Labels`.

## See Also

### Identifying the Argument Encoder

var device: any MTLDevice

The device object that created the argument encoder.

**Required**

