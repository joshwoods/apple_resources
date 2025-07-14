

- FSKit
- FSStatFSResult
-  ioSize 

Instance Property

# ioSize

A property for the optimal block size with which to perform I/O.

macOS 15.4+

``` source
var ioSize: Int { get set }
```

## Discussion

For best performance, specify an `ioSize` that’s an even multiple of blockSize.

