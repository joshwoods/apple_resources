

- System
- Mach
- Mach.Port
-  makeSendCount 

Instance Property

# makeSendCount

Access the make-send count.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.0+watchOS 10.4+

``` source
var makeSendCount: mach_port_mscount_t { get set }
```

Available when `RightType` is `Mach.ReceiveRight`.

## Discussion

Each get/set of this property makes a syscall.

