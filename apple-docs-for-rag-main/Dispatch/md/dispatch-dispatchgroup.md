

- Dispatch
-  DispatchGroup 

Class

# DispatchGroup

A group of tasks that you monitor as a single unit.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class DispatchGroup
```

## Overview

Groups allow you to aggregate a set of tasks and synchronize behaviors on the group. You attach multiple work items to a group and schedule them for asynchronous execution on the same queue or different queues. When all work items finish executing, the group executes its completion handler. You can also wait synchronously for all tasks in the group to finish executing.

## Topics

### Creating a Dispatch Group

init()

Creates a new group to which you can assign block objects.

### Adding a Completion Handler

func notify(qos: DispatchQoS, flags: DispatchWorkItemFlags, queue: DispatchQueue, execute: () -> Void)

Schedules the submission of a block with the specified attributes to a queue when all tasks in the current group have finished executing.

func notify(queue: DispatchQueue, work: DispatchWorkItem)

Schedules the submission of a block to a queue when all tasks in the current group have finished executing.

### Waiting for Tasks to Finish Executing

func wait()

Waits synchronously for the previously submitted work to finish.

func wait(timeout: DispatchTime) -> DispatchTimeoutResult

Waits synchronously for the previously submitted work to complete, and returns if the work is not completed before the specified timeout period has elapsed.

func wait(wallTimeout: DispatchWallTime) -> DispatchTimeoutResult

Waits synchronously for the previously submitted work to complete, and returns if the work is not completed before the specified timeout period has elapsed.

### Updating the Group Manually

func enter()

Explicitly indicates that a block has entered the group.

func leave()

Explicitly indicates that a block in the group finished executing.

## Relationships

### Inherits From

- DispatchObject

### Conforms To

- CVarArg
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Queues and Tasks

class DispatchQueue

An object that manages the execution of tasks serially or concurrently on your app’s main thread or on a background thread.

class DispatchWorkItem

The work you want to perform, encapsulated in a way that lets you attach a completion handle or execution dependencies.

Dispatch Queue

An object that manages the execution of tasks serially or concurrently on your app’s main thread or on a background thread.

Dispatch Work Item

The work you want to perform, encapsulated in a way that lets you attach a completion handle or execution dependencies.

Dispatch Group

A group of tasks that you monitor as a single unit.

Workloop

A dispatch object that prioritizes the execution of tasks based on their quality-of-service (QoS) level.

