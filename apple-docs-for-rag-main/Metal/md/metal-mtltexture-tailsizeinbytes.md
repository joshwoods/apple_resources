

- Metal
- MTLTexture
-  tailSizeInBytes 

Instance Property

# tailSizeInBytes

The size of the sparse texture tail, in bytes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

**iOS, iPadOS, tvOS, visionOS**

``` source
var tailSizeInBytes: Int { get }
```

**Mac Catalyst, macOS**

``` source
optional var tailSizeInBytes: Int { get }
```

**Required**

## See Also

### Querying Sparse Properties

var isSparse: Bool

A Boolean value that indicates whether this is a sparse texture.

**Required**

var firstMipmapInTail: Int

The index of the first mipmap in the tail.

**Required**

