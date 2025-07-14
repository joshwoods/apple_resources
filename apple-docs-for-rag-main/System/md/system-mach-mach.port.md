

- System
- Mach
-  Mach.Port 

Structure

# Mach.Port

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.0+watchOS 10.4+

``` source
struct Port where RightType : MachPortRight
```

## Topics

### Initializers

init()

Allocate a new Mach port with a receive right, creating a Mach.Port\ to manage it.

init(name: mach_port_name_t)

Transfer ownership of an existing unmanaged Mach port right into a `Mach.Port` by name.

init(name: mach_port_name_t, context: mach_port_context_t)

Transfer ownership of an existing, unmanaged, but already guarded, Mach port right into a Mach.Port by name.

init(name: mach_port_name_t, context: mach_port_context_t)

Transfer ownership of an existing, unmanaged, but already guarded, Mach port right into a Mach.Port by name.

### Instance Properties

var makeSendCount: mach_port_mscount_t

Access the make-send count.

### Instance Methods

func copySendRight() throws -> Mach.Port&lt;Mach.SendRight>

Create another send right from a given send right.

func makeSendOnceRight() -> Mach.Port&lt;Mach.SendOnceRight>

Create a send-once right for a given receive right.

func makeSendRight() -> Mach.Port&lt;Mach.SendRight>

Create a send right for a given receive right.

func relinquish() -> mach_port_name_t

Transfer ownership of the underlying port right to the caller.

func relinquish() -> (name: mach_port_name_t, context: mach_port_context_t)

Transfer ownership of the underlying port right to the caller.

func relinquish() -> mach_port_name_t

Transfer ownership of the underlying port right to the caller.

func relinquish() -> (name: mach_port_name_t, context: mach_port_context_t)

Transfer ownership of the underlying port right to the caller.

func unguardAndRelinquish() -> mach_port_name_t

Remove guard and transfer ownership of the underlying port right to the caller.

func withBorrowedName&lt;ReturnType>(body: (mach_port_name_t, mach_port_context_t) -> ReturnType) -> ReturnType

Borrow access to the port name in a block that can perform non-consuming operations.

func withBorrowedName&lt;ReturnType>(body: (mach_port_name_t, mach_port_context_t) -> ReturnType) -> ReturnType

Borrow access to the port name in a block that can perform non-consuming operations.

func withBorrowedName&lt;ReturnType>(body: (mach_port_name_t) -> ReturnType) -> ReturnType

Borrow access to the port name in a block that can perform non-consuming operations.

