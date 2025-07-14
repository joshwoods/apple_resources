

- CarKey
- RemoteKeylessEntryEnduringAction
-  RemoteKeylessEntryEnduringAction.EnduringExecutionRequest Deprecated

Class

# RemoteKeylessEntryEnduringAction.EnduringExecutionRequest

An object that reports the results of an action with an optional stopping point.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.3–15.0DeprecatedwatchOS 9.0–11.0Deprecated

``` source
final class EnduringExecutionRequest
```

Deprecated

Use perform(enduringAction:continuationStrategy:) instead

## Overview

When you perform an action, the system creates a RemoteKeylessEntryEnduringAction.EnduringExecutionRequest object for your request and returns it to your app. Use the object to send a follow-up request to stop the action. You can also use it to determine the status of the original action.

## Topics

### Getting the Vehicle’s Respose

func results() async throws -> ExecutionStatus

Returns the results of a preceding action request.

struct ExecutionStatus

A type that contains the status code a vehicle returns after executing an action.

### Cancelling an Action

func stop() throws

Sends a request to stop a previously started action.

