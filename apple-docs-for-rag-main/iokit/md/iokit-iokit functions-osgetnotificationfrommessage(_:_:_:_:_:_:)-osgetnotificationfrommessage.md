

- IOKit
- IOKit Functions
-  OSGetNotificationFromMessage(\_:\_:\_:\_:\_:\_:) 

Function

# OSGetNotificationFromMessage(\_:\_:\_:\_:\_:\_:)

macOS 10.0+

``` source
func OSGetNotificationFromMessage(
    _ msg: UnsafeMutablePointer!,
    _ index: UInt32,
    _ type: UnsafeMutablePointer!,
    _ reference: UnsafeMutablePointer!,
    _ content: UnsafeMutablePointer!,
    _ size: UnsafeMutablePointer!
) -> kern_return_t
```

