

- WatchKit
-  WKExtendedRuntimeSessionInvalidationReason 

Enumeration

# WKExtendedRuntimeSessionInvalidationReason

The reasons why a session can become invalid.

watchOS 6.0+

``` source
enum WKExtendedRuntimeSessionInvalidationReason
```

## Overview

Sessions become invalid when they encounter an error, or when they stop running.

## Topics

### Invalidation Reasons

case error

An error prevented the session from running.

case none

The session ended normally.

case sessionInProgress

This app already has a running session.

case expired

The session used all of its allocated time.

case resignedFrontmost

The app lost its frontmost status.

case suppressedBySystem

The system is in a state that doesn’t allow sessions of this type.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

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

