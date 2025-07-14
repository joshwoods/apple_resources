

- Foundation
- NSMapTableValueCallBacks
-  describe 

Instance Property

# describe

Points to the function that produces an autoreleased NSString \* describing the given element. If `NULL`, then the map table produces a generic string description.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var describe: ((NSMapTable, UnsafeRawPointer) -> String?)?
```

