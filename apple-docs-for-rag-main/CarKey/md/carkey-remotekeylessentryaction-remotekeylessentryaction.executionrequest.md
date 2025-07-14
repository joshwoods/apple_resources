

- CarKey
- RemoteKeylessEntryAction
-  RemoteKeylessEntryAction.ExecutionRequest 

Class

# RemoteKeylessEntryAction.ExecutionRequest

An object that reports the results of an automatically ending action asynchronously.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.3+watchOS 9.0+

``` source
final class ExecutionRequest
```

## Overview

When you perform an action, the system creates a RemoteKeylessEntryAction.ExecutionRequest object for that request and returns it to your app. Use that object to asynchronously determine whether your request completed successfully or reported an error.

## Topics

### Getting the Vehicle’s Respose

func results() async throws -> ExecutionStatus

Returns the results of a preceding action request.

struct ExecutionStatus

A type that contains the status code a vehicle returns after executing an action.

## Relationships

### Conforms To

- Sendable

