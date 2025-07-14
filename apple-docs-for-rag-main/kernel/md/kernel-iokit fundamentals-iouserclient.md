

- Kernel
- IOKit Fundamentals
-  IOUserClient 

Class

# IOUserClient

Provides a basis for communication between client applications and I/O Kit objects.

macOS 10.0+

``` source
class IOUserClient : IOService
```

## Overview

## Topics

### Miscellaneous

exportObjectToClient

releaseAsyncReference64

Release the mach_port_t reference held within the OSAsyncReference64 structure.

releaseNotificationPort

Release the mach_port_t passed to registerNotificationPort().

removeMappingForDescriptor

sendAsyncResult64WithOptions

Send a notification as with sendAsyncResult, but with finite queueing.

### DataTypes

ExpansionData

### Instance Variables

reserved

### Instance Methods

- AsyncCompletion

- CopyClientEntitlements

- CopyClientEntitlements_Impl

- CopyClientMemoryForType

- CreateActionKernelCompletion

- CreateMemoryDescriptorFromClient

- CreateMemoryDescriptorFromClient_Impl

- Dispatch

- KernelCompletion_Impl

- clientClose

- clientDied

- clientMemoryForType

- clientMemoryForType

- connectClient

- exportObjectToClient

- externalMethod

- free

- getAsyncTargetAndMethodForIndex

- getAsyncTargetAndMethodForIndex

- getExternalAsyncMethodForIndexDeprecated

- getExternalMethodForIndexDeprecated

- getExternalTrapForIndexDeprecated

- getMetaClass

- getNotificationSemaphore

- getService

- getTargetAndMethodForIndex

- getTargetAndMethodForIndex

- getTargetAndTrapForIndex

- init

- init

- initWithTask

- initWithTask

- registerNotificationPort

- registerNotificationPort

- removeMappingForDescriptor

- reserve

### Type Methods

+ AsyncCompletion_Invoke

+ AsyncCompletion_Invoke

+ CopyClientEntitlements_Invoke

+ CopyClientMemoryForType_Invoke

+ CreateMemoryDescriptorFromClient_Invoke

+ clientHasAuthorization

+ clientHasPrivilege

+ copyClientEntitlement

+ copyClientEntitlementVnode

+ copyClientEntitlements

+ copyClientEntitlementsVnode

+ releaseAsyncReference64

+ releaseNotificationPort

+ sendAsyncResult

+ sendAsyncResult64

+ sendAsyncResult64WithOptions

+ setAsyncReference

+ setAsyncReference64

+ setAsyncReference64

## Relationships

### Inherits From

- IOService

## See Also

### User-Space Interactions

IOSharedDataQueue

A generic queue designed to pass data both from the kernel to a user process and from a user process to the kernel.

IOSharedInterruptController

IOStreamUserClient

IOStream

A class representing a stream of data buffers passed from kernel to user space and back again.

IOStreamBuffer

A class representing a data buffer that is part of an IOStream.

OSAction_IOUserClient_KernelCompletion

OSAction_IOUserClient_KernelCompletionInterface

