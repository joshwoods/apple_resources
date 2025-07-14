

- System
- Mach
- Mach.Port
-  init() 

Initializer

# init()

Allocate a new Mach port with a receive right, creating a Mach.Port\ to manage it.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.0+watchOS 10.4+

``` source
init()
```

Available when `RightType` is `Mach.ReceiveRight`.

## Discussion

This initializer will abort if the right could not be created. Callers may assert that a valid right is always returned.

