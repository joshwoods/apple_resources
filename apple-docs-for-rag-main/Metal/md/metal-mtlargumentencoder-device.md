

- Metal
- MTLArgumentEncoder
-  device 

Instance Property

# device

The device object that created the argument encoder.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var device: any MTLDevice { get }
```

**Required**

## Discussion

You can only use the encoder to encode data into buffers created by the same Metal device object.

## See Also

### Identifying the Argument Encoder

var label: String?

A string that identifies the argument buffer.

**Required**

