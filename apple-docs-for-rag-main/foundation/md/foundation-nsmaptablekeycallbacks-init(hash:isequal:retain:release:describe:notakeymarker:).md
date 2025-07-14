

- Foundation
- NSMapTableKeyCallBacks
-  init(hash:isEqual:retain:release:describe:notAKeyMarker:) 

Initializer

# init(hash:isEqual:retain:release:describe:notAKeyMarker:)

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    hash: ((NSMapTable, UnsafeRawPointer) -> Int)?,
    isEqual: ((NSMapTable, UnsafeRawPointer, UnsafeRawPointer) -> ObjCBool)?,
    retain: ((NSMapTable, UnsafeRawPointer) -> Void)?,
    release: ((NSMapTable, UnsafeMutableRawPointer) -> Void)?,
    describe: ((NSMapTable, UnsafeRawPointer) -> String?)?,
    notAKeyMarker: UnsafeRawPointer?
)
```

