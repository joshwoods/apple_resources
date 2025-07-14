

- Foundation
- NSString
-  init(charactersNoCopy:length:deallocator:) 

Initializer

# init(charactersNoCopy:length:deallocator:)

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(
    charactersNoCopy chars: UnsafeMutablePointer,
    length len: Int,
    deallocator: ((UnsafeMutablePointer, Int) -> Void)? = nil
)
```

