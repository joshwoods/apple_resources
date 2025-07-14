

- Foundation
- NSHashTableCallBacks
-  retain 

Instance Property

# retain

Points to the function that increments a reference count for the given element. If `NULL`, then nothing is done for reference counting.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var retain: ((NSHashTable, UnsafeRawPointer) -> Void)?
```

