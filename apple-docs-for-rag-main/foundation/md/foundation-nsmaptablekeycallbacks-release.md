

- Foundation
- NSMapTableKeyCallBacks
-  release 

Instance Property

# release

Points to the function which decrements a reference count for the given element, and if the reference count becomes zero, frees the given element. If `NULL`, then nothing is done for reference counting or releasing.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var release: ((NSMapTable, UnsafeMutableRawPointer) -> Void)?
```

