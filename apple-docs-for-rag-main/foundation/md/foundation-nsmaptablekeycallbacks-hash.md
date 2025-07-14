

- Foundation
- NSMapTableKeyCallBacks
-  hash 

Instance Property

# hash

Points to the function which must produce hash code for key elements of the map table. If `NULL`, the pointer value is used as the hash code. Second parameter is the element for which hash code should be produced.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var hash: ((NSMapTable, UnsafeRawPointer) -> Int)?
```

