

- Foundation
-  MachError 

Structure

# MachError

Describes an error in the Mach error domain.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct MachError
```

## Topics

### Type Aliases

typealias Code

### Type Properties

static var aborted: MachError.Code

The operation was aborted. Ipc code will catch this and reflect it as a message error.

static var alreadyInSet: MachError.Code

The receive right is already a member of the portset.

static var alreadyWaiting: MachError.Code

A thread is attempting to wait for an event for which there is already a waiting thread.

static var codesignError: MachError.Code

During a page fault, indicates that the page was rejected as a result of a signature check.

static var defaultSet: MachError.Code

An attempt was made to destroy the default processor set.

static var exceptionProtected: MachError.Code

An attempt was made to fetch an exception port that is protected, or to abort a thread while processing a protected exception.

static var failure: MachError.Code

The function could not be performed. A catch-all.

static var invalidAddress: MachError.Code

Specified address is not currently valid.

static var invalidArgument: MachError.Code

The function requested was not applicable to this type of argument, or an argument is invalid.

static var invalidCapability: MachError.Code

The supplied (port) capability is improper.

static var invalidHost: MachError.Code

Target host isn’t actually a host.

static var invalidLedger: MachError.Code

A ledger was required but not supplied.

static var invalidMemoryControl: MachError.Code

The port was not a memory cache control port.

static var invalidName: MachError.Code

The name doesn’t denote a right in the task.

static var invalidObject: MachError.Code

The external memory manager failed to initialize the memory object.

static var invalidPolicy: MachError.Code

The specified scheduling policy is not currently enabled for the processor set.

static var invalidProcessorSet: MachError.Code

An argument applied to assert processor set privilege was not a processor set control port.

static var invalidRight: MachError.Code

The name denotes a right, but not an appropriate right.

static var invalidSecurity: MachError.Code

An argument supplied to assert security privilege was not a host security port.

static var invalidTask: MachError.Code

Target task isn’t an active task.

static var invalidValue: MachError.Code

A blatant range error.

static var lockOwned: MachError.Code

The lock is already owned by another thread.

static var lockOwnedSelf: MachError.Code

The lock is already owned by the calling thread.

static var lockSetDestroyed: MachError.Code

Lock set has been destroyed and is no longer available.

static var lockUnstable: MachError.Code

The thread holding the lock terminated before releasing the lock.

static var memoryDataMoved: MachError.Code

A page was requested of a memory manager via memory_object_data_request for an object using a MEMORY_OBJECT_COPY_CALL strategy, with the VM_PROT_WANTS_COPY flag being used to specify that the page desired is for a copy of the object, and the memory manager has detected the page was pushed into a copy of the object while the kernel was walking the shadow chain from the copy to the object. This error code is delivered via memory_object_data_error and is handled by the kernel (it forces the kernel to restart the fault). It will not be seen by users.

static var memoryError: MachError.Code

During a page fault, the memory object indicated that the data could not be returned. This failure may be temporary; future attempts to access this same data may succeed, as defined by the memory object.

static var memoryFailure: MachError.Code

During a page fault, the target address refers to a memory object that has been destroyed. This failure is permanent.

static var memoryPresent: MachError.Code

An attempt was made to supply “precious” data for memory that is already present in a memory object.

static var memoryRestartCopy: MachError.Code

A strategic copy was attempted of an object upon which a quicker copy is now possible. The caller should retry the copy using vm_object_copy_quickly. This error code is seen only by the kernel.

static var nameExists: MachError.Code

The name already denotes a right in the task.

static var noAccess: MachError.Code

Bogus access restriction.

static var noSpace: MachError.Code

The address range specified is already in use, or no address range of the size specified could be found.

static var nodeDown: MachError.Code

Remote node down or inaccessible.

static var notDepressed: MachError.Code

thread_depress_abort was called on a thread which was not currently depressed.

static var notInSet: MachError.Code

The receive right is not a member of a port set.

static var notReceiver: MachError.Code

The task in question does not hold receive rights for the port argument.

static var notSupported: MachError.Code

Empty thread activation (No thread linked to it).

static var notWaiting: MachError.Code

A signalled thread was not actually waiting.

static var operationTimedOut: MachError.Code

Some thread-oriented operation (semaphore_wait) timed out.

static var policyLimit: MachError.Code

The specified scheduling attributes exceed the thread’s limits.

static var policyStatic: MachError.Code

The requested property cannot be changed at this time.

static var protectionFailure: MachError.Code

Specified memory is valid, but does not permit the required forms of access.

static var resourceShortage: MachError.Code

A system resource could not be allocated to fulfill this request. This failure may not be permanent.

static var rightExists: MachError.Code

The task already has send or receive rights for the port under another name.

static var rpcContinueOrphan: MachError.Code

Allow an orphaned activation to continue executing.

static var rpcServerTerminated: MachError.Code

Return from RPC indicating the target server was terminated before it successfully replied.

static var rpcTerminateOrphan: MachError.Code

Terminate an orphaned activation.

static var semaphoreDestroyed: MachError.Code

Semaphore has been destroyed and is no longer available.

static var success: MachError.Code

static var terminated: MachError.Code

Object has been terminated and is no longer available.

static var userReferencesOverflow: MachError.Code

Operation would overflow limit on user-references.

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Error Codes

struct CocoaError

Describes errors within the Cocoa error domain.

struct POSIXError

Describes an error in the POSIX error domain.

NSError Codes

Error codes in the Cocoa error domain.

