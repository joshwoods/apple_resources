

- DriverKit
-  TYPE 

Macro

# TYPE

Annotates a method declaration to indicate that it conforms to an existing method signature.

DriverKitiOSiPadOSmacOS

``` source
#define TYPE(p)
```

## Parameters 

`p`  

The class and method name to which the method conforms. Specify this value using the format `::`. Specify the class and method names directly, and do not use a string.

## Mentioned in 

Creating a Driver Using the DriverKit SDK

## Discussion

Typically, you use this macro to implement DriverKit callbacks using your own custom methods. The macro lets you ignore the original method’s name and choose any name you want. Your method must still declare the same parameters and return type as the original method. For example, the following code shows how to declare a custom version of the DataAvailable method of IODataQueueDispatchSource in your header file.

```
virtual void MyCustomDataAvailable (OSAction *action) TYPE(IODataQueueDispatchSource::DataAvailable);
```

This macro generates the following convenient symbols that you can use when configuring actions involving your custom method:

- A message ID constant you can pass to the Create method of OSAction. The constant takes the form `__ID`. For example, if you add the TYPE macro to the `ReceiveData` method of your custom `MyDriver` class, the corresponding message ID constant is `MyDriver_ReceiveData_ID`.

- A `CreateAction_` function that creates an OSAction object targeting your custom method. For example, if the name of your custom method is `HandleTimer`, the name of the generated function is `CreateActionHandleTimer`.

## See Also

### Runtime support

OSDynamicCast

Casts an object safely to the specified type, if possible.

OSRequiredCast

Casts the object to the specified type, stopping the process if the object isn’t of the correct type.

IMPL

Tells the system that the superclass implementation of this method runs in the kernel.

QUEUENAME

Tells the system to execute a method on the dispatch queue with the specified name.

SUPERDISPATCH

Tells the system to execute the superclass’ implementation of the current method in the kernel.

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

