

- Core Video
- CVPixelBufferLockFlags
-  readOnly 

Type Property

# readOnly

A read-only buffer.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
static var readOnly: CVPixelBufferLockFlags { get }
```

## Discussion

Set this flag if you don’t plan to modify buffer data while holding the lock. Setting this flag improves performance by preventing Core Video from invalidating existing caches of the buffer’s contents.

Important

If you pass this flag to the CVPixelBufferLockBaseAddress(_:_:) function, you must also pass it to the CVPixelBufferUnlockBaseAddress(_:_:) function.

