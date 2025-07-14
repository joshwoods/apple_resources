

- Metal
- MTLTexture
-  isSparse 

Instance Property

# isSparse

A Boolean value that indicates whether this is a sparse texture.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

**Mac Catalyst, macOS**

``` source
optional var isSparse: Bool { get }
```

**iOS, iPadOS, tvOS, visionOS**

``` source
var isSparse: Bool { get }
```

**Required**

## See Also

### Querying Sparse Properties

var firstMipmapInTail: Int

The index of the first mipmap in the tail.

**Required**

var tailSizeInBytes: Int

The size of the sparse texture tail, in bytes.

**Required**

