

- DriverKit
-  LOCAL 

Macro

# LOCAL

Tells the system that the method runs locally in the driver extension’s process space.

DriverKitiOSiPadOSmacOS

``` source
#define LOCAL
```

## Discussion

DriverKit adds this macro to methods that must run locally in your driver extension. A method tagged with this macro may still be called by a remote process such as the kernel. Don’t add this macro to your own methods.

This macro applies only to methods.

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

LOCALONLY

Tells the system that the class or method runs locally in the driver extension’s process space.

Error Codes

Determine the reason an operation fails.

C++ Runtime Support

Examine low-level types that DriverKit uses to support kernel-level operations.

