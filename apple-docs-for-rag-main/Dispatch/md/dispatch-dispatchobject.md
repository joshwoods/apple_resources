

- Dispatch
-  DispatchObject 

Class

# DispatchObject

The base class for most dispatch types.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class DispatchObject
```

## Overview

There are many types of dispatch objects, including DispatchQueue, DispatchGroup, and DispatchSource. The base dispatch object interfaces allow you to manage memory, pause and resume execution, define object context, log task data, and more.

## Topics

### Activating, Suspending, and Resuming

func activate()

Activates the dispatch object.

func resume()

Resumes the invocation of block objects on a dispatch object.

func suspend()

Suspends the invocation of block objects on a dispatch object.

### Changing the Assigned Target Queue

func setTarget(queue: dispatch_queue_t?)

Specifies the dispatch queue on which to perform work associated with the current object.

## Relationships

### Inherits From

- OS_object

### Inherited By

- DispatchGroup
- DispatchIO
- DispatchQueue
- DispatchSemaphore
- DispatchSource

### Conforms To

- CVarArg
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Dispatch Objects

enum DispatchPredicate

Logical conditions to evaluate within a given execution context.

func dispatchPrecondition(condition: @autoclosure () -> DispatchPredicate)

Checks a dispatch condition necessary for further execution.

Dispatch Objects

The basic behaviors supported by all dispatch types.

