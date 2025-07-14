

- Endpoint Security
-  Event Types 

API Collection

# Event Types

Types used by messages to deliver details specific to different kinds of Endpoint Security events.

## Overview

The types in this section contain details of each event that an Endpoint Security message can contain. While the es_message_t type itself is generic, the members of its event union contain specific event types.

For example, when the message’s event_type is ES_EVENT_TYPE_NOTIFY_FORK, you access the event’s fork member, whose type is es_event_fork_t. This type has properties specific to process-forking events, such as the child process that resulted from the fork operation.

## Topics

### File-System Event Types

struct es_file_t

A type that represents a file related to an Endpoint Security event.

struct es_event_access_t

A type for an event that indicates the checking of a file’s access permission.

struct es_event_clone_t

A type for an event that indicates the cloning of a file.

struct es_event_copyfile_t

A type for an event that indicates the copying of a file by use of a system call.

struct es_event_create_t

A type for an event that indicates the creation of a file.

struct es_event_dup_t

A type for an event that indicates the duplication of a file descriptor.

struct es_event_fcntl_t

A type for an event that indicates the manipulation of a file descriptor.

struct es_event_open_t

A type for an event that indicates the opening of a file.

struct es_event_close_t

A type for an event that indicates the closing of a file.

struct es_event_rename_t

A type for an event that indicates the renaming of a file.

struct es_event_truncate_t

A type for an event that indicates the truncation of a file.

struct es_event_exchangedata_t

A type for an event that indicates the exchange of data between two files.

struct es_event_write_t

A type for an event that indicates the writing of data to a file.

struct es_event_lookup_t

A type for an event that indicates the lookup of a file’s path.

struct es_event_searchfs_t

A type for an event that indicates searching a volume or mounted file system.

### File Metadata Event Types

struct es_event_deleteextattr_t

A type for an event that indicates the deletion of an extended attribute from a file.

struct es_event_fsgetpath_t

A type for an event that indicates the retrieval of a file-system path.

struct es_event_getattrlist_t

A type for an event that indicates the retrieval of attributes from a file.

struct es_event_getextattr_t

A type for an event that indicates the retrieval of an extended attribute from a file.

struct es_event_listextattr_t

A type for an event that indicates the retrieval of multiple extended attributes from a file.

struct es_event_readdir_t

A type for an event that indicates the reading of a file-system directory.

struct es_event_setacl_t

A type for an event that indicates the setting of a file’s access control list.

struct es_event_setattrlist_t

A type for an event that indicates the setting of a file attribute.

struct es_event_setextattr_t

A type for an event that indicates the setting of a file’s extended attribute.

struct es_event_setflags_t

A type for an event that indicates the setting of a file’s flags.

struct es_event_setmode_t

A type for an event that indicates the setting of a file’s mode.

struct es_event_setowner_t

A type for an event that indicates the setting of a file’s owner.

struct es_event_stat_t

A type for an event that indicates the retrieval of a file’s status.

struct es_event_utimes_t

A type for an event that indicates a change to a file’s access time or modification time.

### File Provider Event Types

struct es_event_file_provider_materialize_t

A type for an event that indicates the materialization of a file provider.

struct es_event_file_provider_update_t

A type for an event that indicates an update to a file provider.

### Link Event Types

struct es_event_link_t

A type for an event that indicates the creation of a hard link.

struct es_event_readlink_t

A type for an event that indicates the reading of a symbolic link.

struct es_event_unlink_t

A type for an event that indicates the deletion of a file.

### File System Mounting Event Types

struct es_event_mount_t

A type for an event that indicates the mounting of a file system.

struct es_event_unmount_t

A type for an event that indicates the unmounting of a file system.

struct es_event_remount_t

A type for an event that indicates the unmounting of a file system.

### Memory Mapping Event Types

struct es_event_mmap_t

A type for an event that indicates the mapping of memory to a file.

struct es_event_mprotect_t

A type for an event that indicates a change to protection of memory-mapped pages.

### Process Event Types

struct es_event_chdir_t

A type for an event that indicates a change to a process’s working directory.

struct es_event_chroot_t

A type for an event that indicates a change to a process’s root directory.

struct es_event_exec_t

A type for an event that indicates the execution of a process.

struct es_event_fork_t

A type for an event that indicates the forking of a process.

struct es_event_proc_check_t

A type that indicates the call used and the data returned when a process checks on the access of the target process.

struct es_event_signal_t

A type for an event that indicates the sending of a signal to a process.

struct es_event_exit_t

A type for an event that indicates a process exiting.

### Process Event Helper Functions

func es_exec_arg(UnsafePointer&lt;es_event_exec_t>, UInt32) -> es_string_token_t

Gets the argument at the specified position from a process execution event.

func es_exec_arg_count(UnsafePointer&lt;es_event_exec_t>) -> UInt32

Gets the number of arguments from a process execution event.

func es_exec_env(UnsafePointer&lt;es_event_exec_t>, UInt32) -> es_string_token_t

Gets the environment variable at the specified position from a process execution event.

func es_exec_env_count(UnsafePointer&lt;es_event_exec_t>) -> UInt32

Gets the number of environment variables from a process execution event.

func es_exec_fd(UnsafePointer&lt;es_event_exec_t>, UInt32) -> UnsafePointer&lt;es_fd_t>

Gets the file descriptor at the specified position from a process execution event.

func es_exec_fd_count(UnsafePointer&lt;es_event_exec_t>) -> UInt32

Gets the number of file descriptors from a process execution event.

struct es_fd_t

A structure that describes an open file descriptor.

### Interprocess Events

struct es_event_proc_suspend_resume_t

A type for an event that indicates a call to suspend, resume, or shut down sockets for a process.

struct es_event_trace_t

A type for an event that indicates an attempt by one process to attach to another process.

struct es_event_remote_thread_create_t

A type for an event that indicates an attempt by one process to create a thread in another process.

### Task Port Event Types

struct es_event_get_task_t

A type for an event that indicates the retrieval of a task’s control port.

struct es_event_get_task_read_t

A type for an event that indicates the retrieval of a task’s read port.

struct es_event_get_task_inspect_t

A type for an event that indicates the retrieval of a task’s inspect port.

struct es_event_get_task_name_t

A type for an event that indicates the retrieval of a task’s name port.

### User and Group ID Types

struct es_event_setuid_t

A type for an event that indicates the setting of a process’s user ID.

struct es_event_setgid_t

A type for an event that indicates the setting of a process’s group ID.

struct es_event_seteuid_t

A type for an event that indicates the setting of a process’s effective user ID.

struct es_event_setegid_t

A type for an event that indicates the setting of a process’s effective group ID.

struct es_event_setreuid_t

A type for an event that indicates the setting of a process’s real and effective user IDs.

struct es_event_setregid_t

A type for an event that indicates the setting of a process’s real and effective group IDs.

### Code Signing Event Types

struct es_event_cs_invalidated_t

A type for an event that indicates the invalidation of a process’ code signing status.

### Socket Event Types

struct es_event_uipc_bind_t

A type for an event that indicates the binding of a socket to a path.

struct es_event_uipc_connect_t

A type for an event that indicates the connection of a socket.

### Clock Event Types

struct es_event_settime_t

A type for an event that indicates the modification of the system time.

### Kernel Event Types

struct es_event_iokit_open_t

A type for an event that indicates the opening of an IOKit device.

struct es_event_kextload_t

A type for an event that indicates the loading of a kernel extension.

struct es_event_kextunload_t

A type for an event that indicates the unloading of a Kernel Extension (KEXT).

### Pseudoterminal Event Types

struct es_event_pty_close_t

A type for an event that indicates the closing of a pseudoterminal device.

struct es_event_pty_grant_t

A type for an event that indicates the granting of a pseudoterminal device to a user.

## See Also

### Event Monitoring

Client

An opaque type that maintains Endpoint Security client state, and functions related to this type.

Message

A type used by Endpoint Security to notify your client when a monitored action occurs.

