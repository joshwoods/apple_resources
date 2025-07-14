

- Core Media
- CMBlockBufferCustomBlockSource
-  init(version:AllocateBlock:FreeBlock:refCon:) 

Initializer

# init(version:AllocateBlock:FreeBlock:refCon:)

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    version: UInt32,
    AllocateBlock: ((UnsafeMutableRawPointer?, Int) -> UnsafeMutableRawPointer?)?,
    FreeBlock: ((UnsafeMutableRawPointer?, UnsafeMutableRawPointer, Int) -> Void)?,
    refCon: UnsafeMutableRawPointer?
)
```

## See Also

### Initializers

init()

