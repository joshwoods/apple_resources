

- System
- Mach
- Mach.Port
-  makeSendOnceRight() 

Instance Method

# makeSendOnceRight()

Create a send-once right for a given receive right.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.0+watchOS 10.4+

``` source
func makeSendOnceRight() -> Mach.Port
```

Available when `RightType` is `Mach.ReceiveRight`.

## Discussion

This does not affect the makeSendCount of the receive right.

This function will abort if the right could not be created. Callers may assert that a valid right is always returned.

