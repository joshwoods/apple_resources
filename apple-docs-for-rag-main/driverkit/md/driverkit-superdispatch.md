

- DriverKit
-  SUPERDISPATCH 

Macro

# SUPERDISPATCH

Tells the system to execute the superclass’ implementation of the current method in the kernel.

DriverKitiOSiPadOSmacOS

``` source
#define SUPERDISPATCH
```

## Mentioned in 

Creating a Driver Using the DriverKit SDK

## Discussion

When calling the DriverKit implementation of a method that runs in the kernel, use this macro to bridge from your driver extension’s process space to the superclass’ version of the method. You must use this macro to call inherited DriverKit methods annotated with the IIG_KERNEL macro.

To use this macro, call the original method without the `super` prefix and insert this macro as the final parameter in the parameter list. For example, the following code shows how to call the inherited version of the Start method from a custom IOService subclass.

```
kern_return_t IMPL(MyCustomService, Start)
{
   kern_return_t ret;
   ret = Start(provider, SUPERDISPATCH);

   // Other Start code...
}
```

Don’t use this macro when calling the inherited version of a DriverKit method marked with the LOCALONLY macro.

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

IIG_KERNEL

Tells the system that the class or method runs inside the kernel.

LOCAL

Tells the system that the method runs locally in the driver extension’s process space.

LOCALONLY

Tells the system that the class or method runs locally in the driver extension’s process space.

Error Codes

Determine the reason an operation fails.

C++ Runtime Support

Examine low-level types that DriverKit uses to support kernel-level operations.

