

- Endpoint Security
-  es_event_type_t 

Structure

# es_event_type_t

A type used to identify a message’s event type and subscribe to events of that type.

Mac CatalystmacOS

``` source
struct es_event_type_t
```

## Overview

Call the es_subscribe(_:_:_:) function with the constants defined by this type to subscribe to specific Endpoint Security events.

You also use this type when inspecting a received message. The es_message_t member event_type, which is of this type, indicates what kind of event the event field contains.

## Topics

### Authorization Event Types

var ES_EVENT_TYPE_AUTH_CHDIR: es_event_type_t

An identifier for a process that requests permission from the operating system to change the working directory for the process.

var ES_EVENT_TYPE_AUTH_CHROOT: es_event_type_t

An identifier for a process that requests permission from the operating system to change the root directory for the process.

var ES_EVENT_TYPE_AUTH_CLONE: es_event_type_t

An identifier for a process that requests permission from the operating system to clone a file.

var ES_EVENT_TYPE_AUTH_COPYFILE: es_event_type_t

An identifier for a process that requests permission from the operating system to copy a file.

var ES_EVENT_TYPE_AUTH_CREATE: es_event_type_t

An identifier for a process that requests permission from the operating system to create a file.

var ES_EVENT_TYPE_AUTH_DELETEEXTATTR: es_event_type_t

An identifier for a process that requests permission from the operating system to delete an extended attribute from a file.

var ES_EVENT_TYPE_AUTH_EXCHANGEDATA: es_event_type_t

An identifier for a process that requests permission from the operating system to exchange data between two files.

var ES_EVENT_TYPE_AUTH_EXEC: es_event_type_t

An identifier for a process that requests permission from the operating system to execute another image.

var ES_EVENT_TYPE_AUTH_FCNTL: es_event_type_t

An identifier for a process that requests permission from the operating system to manipulate a file descriptor.

var ES_EVENT_TYPE_AUTH_FILE_PROVIDER_MATERIALIZE: es_event_type_t

An identifier for a process that requests permission for a file provider to return a reference to a file.

var ES_EVENT_TYPE_AUTH_FILE_PROVIDER_UPDATE: es_event_type_t

An identifier for a process that requests permission from the operating system to update a file.

var ES_EVENT_TYPE_AUTH_FSGETPATH: es_event_type_t

An identifier for a process that requests permission from the operating system to retrieve a file system path.

var ES_EVENT_TYPE_AUTH_GET_TASK: es_event_type_t

An identifier for a process that requests permission from the operating system to retrieve a process’s task control port.

var ES_EVENT_TYPE_AUTH_GET_TASK_READ: es_event_type_t

An identifier for a process that requests permission from the operating system to retrieve a process’s task read port.

var ES_EVENT_TYPE_AUTH_GETATTRLIST: es_event_type_t

An identifier for a process that requests permission from the operating system to retrieve attributes from a file.

var ES_EVENT_TYPE_AUTH_GETEXTATTR: es_event_type_t

An identifier for a process that requests permission from the operating system to retrieve an extended attribute from a file.

var ES_EVENT_TYPE_AUTH_IOKIT_OPEN: es_event_type_t

An identifier for a process that requests permission from the operating system to open an IOKit device.

var ES_EVENT_TYPE_AUTH_KEXTLOAD: es_event_type_t

An identifier for a process that requests permission from the operating system to load a kernel extension (KEXT).

var ES_EVENT_TYPE_AUTH_LINK: es_event_type_t

An identifier for a process that requests permission from the operating system to create a hard link.

var ES_EVENT_TYPE_AUTH_LISTEXTATTR: es_event_type_t

An identifier for a process that requests permission from the operating system to retrieve multiple extended attributes from a file.

var ES_EVENT_TYPE_AUTH_MMAP: es_event_type_t

An identifier for a process that requests permission from the operating system to map a file into memory.

var ES_EVENT_TYPE_AUTH_MOUNT: es_event_type_t

An identifier for a process that requests permission from the operating system to mount a file system.

var ES_EVENT_TYPE_AUTH_MPROTECT: es_event_type_t

An identifier for a process that requests permission from the operating system to change the protection of memory-mapped pages.

var ES_EVENT_TYPE_AUTH_OPEN: es_event_type_t

An identifier for a process that requests permission from the operating system to open a file.

var ES_EVENT_TYPE_AUTH_PROC_CHECK: es_event_type_t

An identifier for a process that requests permission from the operating system to get information about a process.

var ES_EVENT_TYPE_AUTH_PROC_SUSPEND_RESUME: es_event_type_t

An identifier for a process that requests permission from the operating system to suspend, resume, or shut down sockets for another process.

var ES_EVENT_TYPE_AUTH_READDIR: es_event_type_t

An identifier for a process that requests permission from the operating system to read a file system directory.

var ES_EVENT_TYPE_AUTH_READLINK: es_event_type_t

An identifier for a process that requests permission from the operating system to read a symbolic link.

var ES_EVENT_TYPE_AUTH_REMOUNT: es_event_type_t

An identifier for a process that requests permission from the operating system to mount a file system.

var ES_EVENT_TYPE_AUTH_RENAME: es_event_type_t

An identifier for a process that requests permission from the operating system to rename a file.

var ES_EVENT_TYPE_AUTH_SEARCHFS: es_event_type_t

An identifier for a process that requests permission from the operating system to search a volume or mounted file system.

var ES_EVENT_TYPE_AUTH_SETACL: es_event_type_t

An identifier for a process that requests permission from the operating system to set a file’s access control list.

var ES_EVENT_TYPE_AUTH_SETATTRLIST: es_event_type_t

An identifier for a process that requests permission from the operating system to set attributes of a file.

var ES_EVENT_TYPE_AUTH_SETEXTATTR: es_event_type_t

An identifier for a process that requests permission from the operating system to set an extended attribute of a file.

var ES_EVENT_TYPE_AUTH_SETFLAGS: es_event_type_t

An identifier for a process that requests permission from the operating system to set a file’s flags.

var ES_EVENT_TYPE_AUTH_SETMODE: es_event_type_t

An identifier for a process that requests permission from the operating system to set a file’s mode.

var ES_EVENT_TYPE_AUTH_SETOWNER: es_event_type_t

An identifier for a process that requests permission from the operating system to set a file’s owner.

var ES_EVENT_TYPE_AUTH_SETTIME: es_event_type_t

An identifier for a process that requests permission from the operating system to modify the system time.

var ES_EVENT_TYPE_AUTH_SIGNAL: es_event_type_t

An identifier for a process that requests permission from the operating system to send a signal to a process.

var ES_EVENT_TYPE_AUTH_TRUNCATE: es_event_type_t

An identifier for a process that requests permission from the operating system to truncate a file.

var ES_EVENT_TYPE_AUTH_UIPC_BIND: es_event_type_t

An identifier for a process that requests permission from the operating system to bind a UNIX domain socket.

var ES_EVENT_TYPE_AUTH_UIPC_CONNECT: es_event_type_t

An identifier for a process that requests permission from the operating system to connect a UNIX domain socket.

var ES_EVENT_TYPE_AUTH_UNLINK: es_event_type_t

An identifier for a process that requests permission from the operating system to delete a file.

var ES_EVENT_TYPE_AUTH_UTIMES: es_event_type_t

An identifier for a process that requests permission from the operating system to change a file’s access or modification time.

### Notification Event Types

var ES_EVENT_TYPE_NOTIFY_ACCESS: es_event_type_t

An identifier for a process that notifies endpoint security that it is checking a file’s access permission.

var ES_EVENT_TYPE_NOTIFY_CHDIR: es_event_type_t

An identifier for a process that notifies endpoint security that it is changing the working directory for the process.

var ES_EVENT_TYPE_NOTIFY_CHROOT: es_event_type_t

An identifier for a process that notifies endpoint security that it is changing the root directory for the process.

var ES_EVENT_TYPE_NOTIFY_CLONE: es_event_type_t

An identifier for a process that notifies endpoint security that it is cloning a file.

var ES_EVENT_TYPE_NOTIFY_CLOSE: es_event_type_t

An identifier for a process that notifies endpoint security that it is closing a file.

var ES_EVENT_TYPE_NOTIFY_COPYFILE: es_event_type_t

An identifier for a process that notifies endpoint security that it is copying a file.

var ES_EVENT_TYPE_NOTIFY_CREATE: es_event_type_t

An identifier for a process that notifies endpoint security that it is creating a file.

var ES_EVENT_TYPE_NOTIFY_CS_INVALIDATED: es_event_type_t

An identifier for a process that notifies endpoint security that its code signing status is now invalid.

var ES_EVENT_TYPE_NOTIFY_DELETEEXTATTR: es_event_type_t

An identifier for a process that notifies endpoint security that it is deleting an extended attribute from a file.

var ES_EVENT_TYPE_NOTIFY_DUP: es_event_type_t

An identifier for a process that notifies endpoint security that it is duplicating a file descriptor.

var ES_EVENT_TYPE_NOTIFY_EXCHANGEDATA: es_event_type_t

An identifier for a process that notifies endpoint security that it is exchanging data between two files.

var ES_EVENT_TYPE_NOTIFY_EXEC: es_event_type_t

An identifier for a process that notifies endpoint security that it is executing an image.

var ES_EVENT_TYPE_NOTIFY_EXIT: es_event_type_t

An identifier for a process that notifies endpoint security that it is exiting.

var ES_EVENT_TYPE_NOTIFY_FCNTL: es_event_type_t

An identifier for a process that notifies endpoint security that it is manipulating a file descriptor.

var ES_EVENT_TYPE_NOTIFY_FILE_PROVIDER_MATERIALIZE: es_event_type_t

An identifier for a process that notifies endpoint security that a file provider returned a reference to a file.

var ES_EVENT_TYPE_NOTIFY_FILE_PROVIDER_UPDATE: es_event_type_t

An identifier for a process that notifies endpoint security that it is updating a file.

var ES_EVENT_TYPE_NOTIFY_FORK: es_event_type_t

An identifier for a process that notifies endpoint security that it is forking another process.

var ES_EVENT_TYPE_NOTIFY_FSGETPATH: es_event_type_t

An identifier for a process that notifies endpoint security that it is retrieving a file system path.

var ES_EVENT_TYPE_NOTIFY_GETATTRLIST: es_event_type_t

An identifier for a process that notifies endpoint security that it is retrieving attributes from a file.

var ES_EVENT_TYPE_NOTIFY_GETEXTATTR: es_event_type_t

An identifier for a process that notifies endpoint security that it is retrieving an extended attribute from a file.

var ES_EVENT_TYPE_NOTIFY_GET_TASK: es_event_type_t

An identifier for a process that notifies endpoint security that it is retrieving the task control port for another process.

var ES_EVENT_TYPE_NOTIFY_GET_TASK_READ: es_event_type_t

An identifier for a process that notifies endpoint security that it is retrieving the task read port for another process.

var ES_EVENT_TYPE_NOTIFY_GET_TASK_INSPECT: es_event_type_t

An identifier for a process that notifies endpoint security that it is retrieving the task inspect port for another process.

var ES_EVENT_TYPE_NOTIFY_GET_TASK_NAME: es_event_type_t

An identifier for a process that notifies endpoint security that it is retrieving the task name port for another process.

var ES_EVENT_TYPE_NOTIFY_IOKIT_OPEN: es_event_type_t

An identifier for a process that notifies endpoint security that it is opening an IOKit device.

var ES_EVENT_TYPE_NOTIFY_KEXTLOAD: es_event_type_t

An identifier for a process that notifies endpoint security that it is loading a kernel extension (KEXT).

var ES_EVENT_TYPE_NOTIFY_KEXTUNLOAD: es_event_type_t

An identifier for a process that notifies endpoint security that it is unloading a kernel extension (KEXT).

var ES_EVENT_TYPE_NOTIFY_LINK: es_event_type_t

An identifier for a process that notifies endpoint security that it is creating a hard link.

var ES_EVENT_TYPE_NOTIFY_LISTEXTATTR: es_event_type_t

An identifier for a process that notifies endpoint security that it is retrieving multiple extended attributes from a file.

var ES_EVENT_TYPE_NOTIFY_LOOKUP: es_event_type_t

An identifier for a process that notifies endpoint security that it is looking up a file’s path.

var ES_EVENT_TYPE_NOTIFY_MMAP: es_event_type_t

An identifier for a process that notifies endpoint security that it is mapping a file into memory.

var ES_EVENT_TYPE_NOTIFY_MOUNT: es_event_type_t

An identifier for a process that notifies endpoint security that it is mounting a file system.

var ES_EVENT_TYPE_NOTIFY_MPROTECT: es_event_type_t

An identifier for a process that notifies endpoint security that it is changing the protection of memory-mapped pages.

var ES_EVENT_TYPE_NOTIFY_OPEN: es_event_type_t

An identifier for a process that notifies endpoint security that it is opening a file.

var ES_EVENT_TYPE_NOTIFY_PROC_CHECK: es_event_type_t

An identifier for a process that notifies endpoint security that it is checking information about another process.

var ES_EVENT_TYPE_NOTIFY_PROC_SUSPEND_RESUME: es_event_type_t

An identifier for a process that notifies endpoint security that it is suspending, resuming, or shutting down sockets for another process.

var ES_EVENT_TYPE_NOTIFY_PTY_CLOSE: es_event_type_t

An identifier for a process that notifies endpoint security that it is closing a pseudoterminal device.

var ES_EVENT_TYPE_NOTIFY_PTY_GRANT: es_event_type_t

An identifier for a process that notifies endpoint security that it is granting a pseudoterminal device to a user.

var ES_EVENT_TYPE_NOTIFY_READDIR: es_event_type_t

An identifier for a process that notifies endpoint security that it is reading a file system directory.

var ES_EVENT_TYPE_NOTIFY_READLINK: es_event_type_t

An identifier for a process that notifies endpoint security that it is reading a symbolic link.

var ES_EVENT_TYPE_NOTIFY_REMOTE_THREAD_CREATE: es_event_type_t

An identifier for a process that notifies endpoint security that it is spawning a thread in another process.

var ES_EVENT_TYPE_NOTIFY_REMOUNT: es_event_type_t

An identifier for a process that notifies endpoint security that it is remounting a file system.

var ES_EVENT_TYPE_NOTIFY_RENAME: es_event_type_t

An identifier for a process that notifies endpoint security that it is renaming a file.

var ES_EVENT_TYPE_NOTIFY_SEARCHFS: es_event_type_t

An identifier for a process that notifies endpoint security that it is searching a volume or mounted file system.

var ES_EVENT_TYPE_NOTIFY_SETACL: es_event_type_t

An identifier for a process that notifies endpoint security that it is setting a file’s access control list.

var ES_EVENT_TYPE_NOTIFY_SETATTRLIST: es_event_type_t

An identifier for a process that notifies endpoint security that it is setting attributes of a file.

var ES_EVENT_TYPE_NOTIFY_SETEGID: es_event_type_t

An identifier for a process that notifies endpoint security that it is setting its effective group ID.

var ES_EVENT_TYPE_NOTIFY_SETEUID: es_event_type_t

An identifier for a process that notifies endpoint security that it is setting its effective user ID.

var ES_EVENT_TYPE_NOTIFY_SETEXTATTR: es_event_type_t

An identifier for a process that notifies endpoint security that it is setting an extended attribute of a file.

var ES_EVENT_TYPE_NOTIFY_SETGID: es_event_type_t

An identifier for a process that notifies endpoint security that it is setting its group ID.

var ES_EVENT_TYPE_NOTIFY_SETFLAGS: es_event_type_t

An identifier for a process that notifies endpoint security that it is setting a file’s flags.

var ES_EVENT_TYPE_NOTIFY_SETMODE: es_event_type_t

An identifier for a process that notifies endpoint security that it is setting a file’s mode.

var ES_EVENT_TYPE_NOTIFY_SETOWNER: es_event_type_t

An identifier for a process that notifies endpoint security that it is setting a file’s owner.

var ES_EVENT_TYPE_NOTIFY_SETREGID: es_event_type_t

An identifier for a process that notifies endpoint security that it is setting its real and effective group IDs.

var ES_EVENT_TYPE_NOTIFY_SETREUID: es_event_type_t

An identifier for a process that notifies endpoint security that it is setting its real and effective user IDs.

var ES_EVENT_TYPE_NOTIFY_SETTIME: es_event_type_t

An identifier for a process that notifies endpoint security that it is modifying the system time.

var ES_EVENT_TYPE_NOTIFY_SETUID: es_event_type_t

An identifier for a process that notifies endpoint security that it is setting its user ID.

var ES_EVENT_TYPE_NOTIFY_SIGNAL: es_event_type_t

An identifier for a process that notifies endpoint security that it is sending a signal to another process.

var ES_EVENT_TYPE_NOTIFY_STAT: es_event_type_t

An identifier for a process that notifies endpoint security that it is retrieving a file’s status.

var ES_EVENT_TYPE_NOTIFY_TRACE: es_event_type_t

An identifier for a process that notifies endpoint security that it is attaching to another process.

var ES_EVENT_TYPE_NOTIFY_TRUNCATE: es_event_type_t

An identifier for a process that notifies endpoint security that it is truncating a file.

var ES_EVENT_TYPE_NOTIFY_UIPC_BIND: es_event_type_t

An identifier for a process that notifies endpoint security that it is binding a UNIX domain socket.

var ES_EVENT_TYPE_NOTIFY_UIPC_CONNECT: es_event_type_t

An identifier for a process that notifies endpoint security that it is connecting to a UNIX domain socket.

var ES_EVENT_TYPE_NOTIFY_UNLINK: es_event_type_t

An identifier for a process that notifies endpoint security that it is deleting a file.

var ES_EVENT_TYPE_NOTIFY_UNMOUNT: es_event_type_t

An identifier for a process that notifies endpoint security that it is unmounting a file system.

var ES_EVENT_TYPE_NOTIFY_UTIMES: es_event_type_t

An identifier for a process that notifies endpoint security that it is changing a file’s access or modification time.

var ES_EVENT_TYPE_NOTIFY_WRITE: es_event_type_t

An identifier for a process that notifies endpoint security that it is writing data to a file.

### Enumeration Marker

var ES_EVENT_TYPE_LAST: es_event_type_t

A value that indicates the last member of the enumeration.

### Initializers

init(UInt32)

init(rawValue: UInt32)

### Instance Properties

var rawValue: UInt32

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Subscribing to Events

func es_subscribe(OpaquePointer, UnsafePointer&lt;es_event_type_t>, UInt32) -> es_return_t

Subscribes a client to a set of events.

func es_subscriptions(OpaquePointer, UnsafeMutablePointer&lt;Int>, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;es_event_type_t>>?) -> es_return_t

Returns a list of the client’s subscriptions.

func es_unsubscribe(OpaquePointer, UnsafePointer&lt;es_event_type_t>, UInt32) -> es_return_t

Unsubscribes the provided client from a set of events.

func es_unsubscribe_all(OpaquePointer) -> es_return_t

Unsubscribes a client from all events.

