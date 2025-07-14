

- Endpoint Security
-  es_message_t 

Structure

# es_message_t

A message from the Endpoint Security subsystem that describes a security event.

Mac CatalystmacOS

``` source
struct es_message_t
```

## Overview

A message contains an event monitored by Endpoint Security and an action to perform. The event is a union of types specific to each kind of event. For example, a file-renaming event provides the source and destination paths as the union member `rename`. Similarly, a process fork event provides the process identifier of the new child process as the union member `fork`. Inspect the event_type to determine which member of the union to access.

A message can be an authorization request, or a notification of an event that has already taken place, as indicated by the action_type field. For authorization messages, your client handler calls es_respond_auth_result(_:_:_:_:) or es_respond_flags_result(_:_:_:_:) to authorize, deny, or pass behavior flags back to Endpoint Security.

## Topics

### Inspecting Message Properties

var action: es_message_t.__Unnamed_union_action

The action monitored by Endpoint Security.

var action_type: es_action_type_t

The type of action: authentication or notification.

struct es_action_type_t

The type of the message’s action.

struct es_event_id_t

An opaque identifier for events.

struct es_result_t

The result of the Endpoint Security subsystem authorization process.

var version: UInt32

The version of the Endpoint Security message.

### Identifying the Matched Event

var event: es_events_t

The event that triggered this message.

struct es_events_t

A C union of event-specific types.

var event_type: es_event_type_t

The type of the message’s event.

struct es_event_type_t

A type used to identify a message’s event type and subscribe to events of that type.

### Inspecting Timing Properties

var time: timespec

The time the event occurred, expressed as a Darwin time value.

var mach_time: UInt64

The time the event occurred, as a Mach time value.

var deadline: UInt64

The deadline by which your app must respond to the event.

var seq_num: UInt64

The sequence number of the message.

var global_seq_num: UInt64

The global sequence number of the message.

### Identifying the Source Process

var process: UnsafeMutablePointer&lt;es_process_t>

The process that performed the action defined in a message.

struct es_process_t

A type that describes a process, as delivered by an Endpoint Security message.

### Inspecting Thread Properties

var thread: UnsafeMutablePointer&lt;es_thread_t>?

The thread that took the action defined in a message.

struct es_thread_t

A structure that represents a thread in a process.

