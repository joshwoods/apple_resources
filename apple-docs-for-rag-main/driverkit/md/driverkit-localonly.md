

- DriverKit
-  LOCALONLY 

Macro

# LOCALONLY

Tells the system that the class or method runs locally in the driver extension’s process space.

DriverKitiOSiPadOSmacOS

``` source
#define LOCALONLY
```

## Discussion

DriverKit adds this macro to classes and methods that cannot be called remotely by the kernel or other processes. Instead, you call the methods locally from your driver’s process space. When applied to a class, the macro affects all methods of that class.

When calling the superclass implementation of a local-only method, call `super` like you normally would. Don’t use the SUPERDISPATCH macro to call the inherited implementation.

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

IIG_KERNEL

Tells the system that the class or method runs inside the kernel.

LOCAL

Tells the system that the method runs locally in the driver extension’s process space.

Error Codes

Determine the reason an operation fails.

C++ Runtime Support

Examine low-level types that DriverKit uses to support kernel-level operations.

