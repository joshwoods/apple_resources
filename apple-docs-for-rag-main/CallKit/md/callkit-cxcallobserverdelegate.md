

- CallKit
-  CXCallObserverDelegate 

Protocol

# CXCallObserverDelegate

A collection of methods the system calls when a call changes state.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
protocol CXCallObserverDelegate : NSObjectProtocol
```

## Topics

### Responding to Changes in Call State

func callObserver(CXCallObserver, callChanged: CXCall)

Called when a call is changed.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Call information

class CXCall

A telephony call.

class CXCallObserver

A programmatic interface for an object that manages a list of active calls and observes call changes.

class CXHandle

A way to reach a call recipient, such as a phone number or email address.

