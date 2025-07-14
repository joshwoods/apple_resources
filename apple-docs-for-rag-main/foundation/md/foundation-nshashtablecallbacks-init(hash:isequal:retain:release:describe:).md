

- Foundation
- NSHashTableCallBacks
-  init(hash:isEqual:retain:release:describe:) 

Initializer

# init(hash:isEqual:retain:release:describe:)

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    hash: ((NSHashTable, UnsafeRawPointer) -> Int)?,
    isEqual: ((NSHashTable, UnsafeRawPointer, UnsafeRawPointer) -> ObjCBool)?,
    retain: ((NSHashTable, UnsafeRawPointer) -> Void)?,
    release: ((NSHashTable, UnsafeMutableRawPointer) -> Void)?,
    describe: ((NSHashTable, UnsafeRawPointer) -> String?)?
)
```

