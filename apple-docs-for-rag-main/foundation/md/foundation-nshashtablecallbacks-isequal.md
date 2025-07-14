

- Foundation
- NSHashTableCallBacks
-  isEqual 

Instance Property

# isEqual

Points to the function that compares second and third parameters. If `NULL`, then == is used for comparison.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isEqual: ((NSHashTable, UnsafeRawPointer, UnsafeRawPointer) -> ObjCBool)?
```

