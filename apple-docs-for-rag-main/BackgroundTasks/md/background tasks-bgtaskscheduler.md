

- Background Tasks
-  BGTaskScheduler 

Class

# BGTaskScheduler

A class for scheduling task requests that launch your app in the background.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
class BGTaskScheduler
```

## Overview

Background tasks give your app a way to run code while the app is suspended. To learn how to register, schedule, and run a background task, see Using background tasks to update your app.

## Topics

### Getting the shared task scheduler

class var shared: BGTaskScheduler

The shared background task scheduler instance.

### Scheduling a task

func register(forTaskWithIdentifier: String, using: dispatch_queue_t?, launchHandler: (BGTask) -> Void) -> Bool

Register a launch handler for the task with the associated identifier that’s executed on the specified queue.

func submit(BGTaskRequest) throws

Submit a previously registered background task for execution.

### Canceling a task

func cancel(taskRequestWithIdentifier: String)

Cancel a previously scheduled task request.

func cancelAllTaskRequests()

Cancel all scheduled task requests.

### Getting all scheduled tasks

func getPendingTaskRequests(completionHandler: ([BGTaskRequest]) -> Void)

Request a list of unexecuted scheduled task requests.

### Handling errors

struct Error

The Errors for the `BGTaskSchedulerError` domain.

enum Code

An enumeration of the task scheduling errors.

class let errorDomain: String

The background tasks error domain as a string.

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

### Essentials

Starting and Terminating Tasks During Development

Use the debugger during development to start tasks and to terminate them before completion.

Refreshing and Maintaining Your App Using Background Tasks

Use scheduled background tasks for refreshing your app content and for performing maintenance.

Choosing Background Strategies for Your App

Select the best method of scheduling background runtime for your app.

