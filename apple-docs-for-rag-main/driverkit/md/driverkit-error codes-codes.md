

- DriverKit
-  Error Codes 

API Collection

# Error Codes

Determine the reason an operation fails.

## Topics

### No Error

kIOReturnSuccess

### Errors

kIOReturnAborted

kIOReturnBadArgument

kIOReturnBadMedia

kIOReturnBadMessageID

kIOReturnBusy

kIOReturnCannotLock

kIOReturnCannotWire

kIOReturnDeviceError

kIOReturnDMAError

kIOReturnError

kIOReturnExclusiveAccess

kIOReturnInternalError

kIOReturnInvalid

kIOReturnIOError

kIOReturnIPCError

kIOReturnIsoTooNew

kIOReturnIsoTooOld

kIOReturnLockedRead

kIOReturnLockedWrite

kIOReturnMessageTooLarge

kIOReturnNoBandwidth

kIOReturnNoChannels

kIOReturnNoCompletion

kIOReturnNoDevice

kIOReturnNoFrames

kIOReturnNoInterrupt

kIOReturnNoMedia

kIOReturnNoMemory

kIOReturnNoPower

kIOReturnNoResources

kIOReturnNoSpace

kIOReturnNotAligned

kIOReturnNotAttached

kIOReturnNotFound

kIOReturnNotOpen

kIOReturnNotPermitted

kIOReturnNotPrivileged

kIOReturnNotReadable

kIOReturnNotReady

kIOReturnNotResponding

kIOReturnNotWritable

kIOReturnOffline

kIOReturnOverrun

kIOReturnPortExists

kIOReturnRLDError

kIOReturnStillOpen

kIOReturnTimeout

kIOReturnUnderrun

kIOReturnUnformattedMedia

kIOReturnUnsupported

kIOReturnUnsupportedMode

kIOReturnVMError

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

LOCALONLY

Tells the system that the class or method runs locally in the driver extension’s process space.

C++ Runtime Support

Examine low-level types that DriverKit uses to support kernel-level operations.

