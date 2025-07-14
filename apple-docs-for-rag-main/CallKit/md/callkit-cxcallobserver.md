

- CallKit
-  CXCallObserver 

Class

# CXCallObserver

A programmatic interface for an object that manages a list of active calls and observes call changes.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
class CXCallObserver
```

## Overview

You can retrieve a list of active calls on an CXCallObserver object using the calls property. You can also provide an object conforming to the CXCallObserverDelegate protocol as the call observer delegate using the setDelegate(_:queue:) method to respond to any active call changes.

VoIP apps typically interact with the CXCallObserver object returned by the callObserver property of a CXCallController instance. However, any app can create a new CXCallObserver object to be notified of any calls activity on the system.

## Topics

### Setting a Delegate

func setDelegate((any CXCallObserverDelegate)?, queue: dispatch_queue_t?)

Sets a call observer delegate, specifying an optional queue on which to execute delegate methods.

### Accessing Calls

var calls: [CXCall]

Returns the active calls of the telephony provider.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Call information

class CXCall

A telephony call.

protocol CXCallObserverDelegate

A collection of methods the system calls when a call changes state.

class CXHandle

A way to reach a call recipient, such as a phone number or email address.

