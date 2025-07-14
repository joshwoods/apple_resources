

- System
- Mach
- Mach.Port
-  withBorrowedName(body:) 

Instance Method

# withBorrowedName(body:)

Borrow access to the port name in a block that can perform non-consuming operations.

iOS 17.4+iPadOS 17.4+macOS 14.4+tvOS 17.4+watchOS 10.4+

``` source
func withBorrowedName(body: (mach_port_name_t, mach_port_context_t) -> ReturnType) -> ReturnType
```

Available when `RightType` is `Mach.ReceiveRight`.

## Discussion

Take care when using this function; many operations consume rights.

If the right is consumed, behavior is undefined.

The body block may optionally return something, which will then be returned to the caller of withBorrowedName.

