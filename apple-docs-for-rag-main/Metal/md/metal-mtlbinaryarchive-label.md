

- Metal
- MTLBinaryArchive
-  label 

Instance Property

# label

A string that identifies the library.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var label: String? { get set }
```

**Required**

## Discussion

Object and command labels are useful identifiers at runtime or when profiling and debugging your app using any Metal tool. See `Enhancing Frame Capture by Using Labels`.

## See Also

### Identifying the Archive

var device: any MTLDevice

The Metal device object that created the binary archive.

**Required**

