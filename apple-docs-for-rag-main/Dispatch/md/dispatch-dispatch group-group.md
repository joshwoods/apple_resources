

- Dispatch
-  Dispatch Group 

API Collection

# Dispatch Group

A group of tasks that you monitor as a single unit.

## Overview

Groups allow you to aggregate a set of tasks and synchronize behaviors on the group. You attach multiple blocks to a group and schedule them for asynchronous execution on the same queue or different queues. When all blocks finish executing, the group executes its completion handler. You can also wait synchronously for all blocks in the group to finish executing.

## Topics

### Creating a Dispatch Group

init()

Creates a new group to which you can assign block objects.

typealias dispatch_group_t

A group of block objects submitted to a queue for asynchronous invocation.

### Updating the Group Manually

func enter()

Explicitly indicates that a block has entered the group.

func leave()

Explicitly indicates that a block in the group finished executing.

## See Also

### Queues and Tasks

class DispatchQueue

An object that manages the execution of tasks serially or concurrently on your app’s main thread or on a background thread.

class DispatchWorkItem

The work you want to perform, encapsulated in a way that lets you attach a completion handle or execution dependencies.

class DispatchGroup

A group of tasks that you monitor as a single unit.

Dispatch Queue

An object that manages the execution of tasks serially or concurrently on your app’s main thread or on a background thread.

Dispatch Work Item

The work you want to perform, encapsulated in a way that lets you attach a completion handle or execution dependencies.

Workloop

A dispatch object that prioritizes the execution of tasks based on their quality-of-service (QoS) level.

