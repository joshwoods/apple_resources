

- Metal
- MTLTexture
-  firstMipmapInTail 

Instance Property

# firstMipmapInTail

The index of the first mipmap in the tail.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

**iOS, iPadOS, tvOS, visionOS**

``` source
var firstMipmapInTail: Int { get }
```

**Mac Catalyst, macOS**

``` source
optional var firstMipmapInTail: Int { get }
```

**Required**

## Discussion

In a sparse texture, the *tail* is a collection of mipmaps at higher index values that are mapped as a single block of memory. When you map this mipmap into your sparse texture, Metal also maps mipmap levels with larger index values.

## See Also

### Querying Sparse Properties

var isSparse: Bool

A Boolean value that indicates whether this is a sparse texture.

**Required**

var tailSizeInBytes: Int

The size of the sparse texture tail, in bytes.

**Required**

