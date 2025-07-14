

- CarKey
- RemoteKeylessEntryConfigurableEnduringAction
-  RemoteKeylessEntryConfigurableEnduringAction.EnduringExecutionRequest 

Class

# RemoteKeylessEntryConfigurableEnduringAction.EnduringExecutionRequest

An object that reports the results of an action with an optional stopping point.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+watchOS 11.0+

``` source
@objc
final class EnduringExecutionRequest
```

## Overview

When you perform an action, the system creates a RemoteKeylessEntryConfigurableEnduringAction.EnduringExecutionRequest object for your request and returns it to your app. Use the object to send a follow-up request to stop the action. You can also use it to determine the status of the original action.

## Topics

### Structures

struct ContinuationRequest

Continuation Request

### Instance Properties

var eventStream: AsyncStream&lt;RemoteKeylessEntryConfigurableEnduringAction.EnduringExecutionRequest.Event>

The asynchronous event stream on which Continuation Requests are sent

### Instance Methods

func results() async throws -> ExecutionStatus

Returns the results of a preceding action request.

func stop() throws

Sends a request to stop a previously started action.

### Enumerations

enum Event

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

