

- DriverKit
-  IIG_KERNEL 

Macro

# IIG_KERNEL

Tells the system that the class or method runs inside the kernel.

DriverKitiOSiPadOSmacOS

``` source
#define IIG_KERNEL
```

## Discussion

DriverKit adds this macro to methods that must run inside the kernel’s process space. When overriding a method tagged with this macro, you must define your method using the IMPL macro, which creates the necessary binding to bridge from your driver’s process space to the kernel implementation. When applied to a class, this macro affects all methods of the class.

Don’t apply this macro to your own classes and methods.

## See Also

### Runtime support

OSDynamicCast

Casts an object safely to the specified type, if possible.

OSRequiredCast

Casts the object to the specified type, stopping the process if the object isn’t of the correct type.

IMPL

Tells the system that the superclass implementation of this method runs in the kernel.

TYPE

Annotates a method declaration to indicate that it conforms to an existing method signature.

QUEUENAME

Tells the system to execute a method on the dispatch queue with the specified name.

SUPERDISPATCH

Tells the system to execute the superclass’ implementation of the current method in the kernel.

LOCAL

Tells the system that the method runs locally in the driver extension’s process space.

LOCALONLY

Tells the system that the class or method runs locally in the driver extension’s process space.

Error Codes

Determine the reason an operation fails.

C++ Runtime Support

Examine low-level types that DriverKit uses to support kernel-level operations.

