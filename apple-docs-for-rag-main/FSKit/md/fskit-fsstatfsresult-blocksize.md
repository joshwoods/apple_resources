

- FSKit
- FSStatFSResult
-  blockSize 

Instance Property

# blockSize

A property for the volume’s block size, in bytes.

macOS 15.4+

``` source
var blockSize: Int { get set }
```

## Discussion

This value defaults to `4096`. Zero isn’t a valid block size.

