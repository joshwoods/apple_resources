

- WatchKit
-  WKExtendedRuntimeSessionDelegate 

Protocol

# WKExtendedRuntimeSessionDelegate

A set of optional methods for monitoring an extended runtime session.

watchOS 6.0+

``` source
protocol WKExtendedRuntimeSessionDelegate : NSObjectProtocol
```

## Mentioned in 

Using extended runtime sessions

## Overview

Implement these methods to track the changes to your session’s state.

## Topics

### Monitoring State Changes

func extendedRuntimeSessionDidStart(WKExtendedRuntimeSession)

Indicates that the session has started running.

**Required**

func extendedRuntimeSessionWillExpire(WKExtendedRuntimeSession)

Indicates that the session is about to expire.

**Required**

func extendedRuntimeSession(WKExtendedRuntimeSession, didInvalidateWith: WKExtendedRuntimeSessionInvalidationReason, error: (any Error)?)

Indicates that the session has encountered an error or stopped running.

**Required**

enum WKExtendedRuntimeSessionInvalidationReason

The reasons why a session can become invalid.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Creating a Session

var delegate: (any WKExtendedRuntimeSessionDelegate)?

A delegate object for monitoring the session and responding to state changes and errors.

