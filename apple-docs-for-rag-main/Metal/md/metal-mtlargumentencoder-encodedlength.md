

- Metal
- MTLArgumentEncoder
-  encodedLength 

Instance Property

# encodedLength

The number of bytes required to store the encoded resources of an argument buffer.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var encodedLength: Int { get }
```

**Required**

## Discussion

After creating a MTLArgumentEncoder object, use this value to create the MTLBuffer object that represents an argument buffer.

```
id  encoder = [_function newArgumentEncoderWithBufferIndex:0];
id  buffer = [_device newBufferWithLength:encoder.encodedLength options:_options];
[encoder setArgumentBuffer:buffer offset:0];
```

## See Also

### Creating an Argument Buffer

func setArgumentBuffer((any MTLBuffer)?, offset: Int)

Specifies the position in a buffer where the encoder writes argument data.

**Required**

func setArgumentBuffer((any MTLBuffer)?, startOffset: Int, arrayElement: Int)

Specifies an array element within a buffer where the encoder writes argument data.

**Required**

