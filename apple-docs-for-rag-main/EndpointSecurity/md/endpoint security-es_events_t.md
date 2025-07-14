

- Endpoint Security
-  es_events_t 

Structure

# es_events_t

A C union of event-specific types.

Mac CatalystmacOS

``` source
struct es_events_t
```

## Overview

Each event monitored by Endpoint Security delivers different properties to clients. For example, a file-renaming event provides source and target paths, while a process-forking event provides the process identifier of the new child process. This C `union` represents each kind of event as a unique member, each with a type specific to the kind of data it contains.

## Topics

### File-System Events

var access: es_event_access_t

Properties of an event that indicates the checking of a file’s access permission.

var clone: es_event_clone_t

Properties of an event that indicates the cloning of a file.

var copyfile: es_event_copyfile_t

Properties of an event that indicates the cloning of a file.

var close: es_event_close_t

Properties of an event that indicates the closing of a file.

var create: es_event_create_t

Properties of an event that indicates the creation of a file.

var dup: es_event_dup_t

Properties of an event that indicates the duplication of a file descriptor.

var exchangedata: es_event_exchangedata_t

Properties of an event that indicates the exchange of data between two files.

var fcntl: es_event_fcntl_t

Properties of an event that indicates the manipulation of a file descriptor.

var open: es_event_open_t

Properties of an event that indicates the opening of a file.

var rename: es_event_rename_t

Properties of an event that indicates the renaming of a file.

var write: es_event_write_t

Properties of an event that indicates the writing of data to a file.

var truncate: es_event_truncate_t

Properties of an event that indicates the truncation of a file.

var lookup: es_event_lookup_t

Properties of an event that indicates the lookup of a file’s path.

var searchfs: es_event_searchfs_t

Properties of an event that indicates a search operation on a volume or mounted file system.

### File Metadata Events

var deleteextattr: es_event_deleteextattr_t

Properties of an event that indicates the deletion of an extended attribute from a file.

var fsgetpath: es_event_fsgetpath_t

Properties of an event that indicates the retrieval of a file-system path.

var getattrlist: es_event_getattrlist_t

Properties of an event that indicates the retrieval of attributes from a file.

var getextattr: es_event_getextattr_t

Properties of an event that indicates the retrieval of an extended attribute from a file.

var listextattr: es_event_listextattr_t

Properties of an event that indicates the retrieval of multiple extended attributes from a file.

var readdir: es_event_readdir_t

Properties of an event that indicates the reading of a file-system directory.

var setacl: es_event_setacl_t

Properties of an event that indicates the setting of a file’s access control list.

var setattrlist: es_event_setattrlist_t

Properties of an event that indicates the setting of an attribute of a file.

var setextattr: es_event_setextattr_t

Properties of an event that indicates the setting of an extended attribute of a file.

var setflags: es_event_setflags_t

Properties of an event that indicates the setting of a file’s flags.

var setmode: es_event_setmode_t

Properties of an event that indicates the setting of a file’s mode.

var setowner: es_event_setowner_t

Properties of an event that indicates the setting of a file’s owner.

var stat: es_event_stat_t

Properties of an event that indicates the retrieval of a file’s status.

var utimes: es_event_utimes_t

Properties of an event that indicates a change to a file’s access time or modification time.

### File Provider Events

var file_provider_materialize: es_event_file_provider_materialize_t

Properties of an event that indicates the materialization of a file provider.

var file_provider_update: es_event_file_provider_update_t

Properties of an event that indicates an update to a file provider.

### Symbolic Link Events

var link: es_event_link_t

Properties of an event that indicates the creation of a hard link.

var readlink: es_event_readlink_t

Properties of an event that indicates the reading of a symbolic link.

var unlink: es_event_unlink_t

Properties of an event that indicates the deletion of a file.

### File System Mounting Events

var mount: es_event_mount_t

Properties of an event that indicates the mounting of a file system.

var unmount: es_event_unmount_t

Properties of an event that indicates the unmounting of a file system.

var remount: es_event_remount_t

Properties of an event that indicates the remounting of a file system.

### Memory Mapping Events

var mmap: es_event_mmap_t

Properties of an event that indicates the mapping of memory to a file.

var mprotect: es_event_mprotect_t

Properties of an event that indicates a change to protection of memory-mapped pages.

### Process Events

var chdir: es_event_chdir_t

Properties of an event that indicates a change to a process’s working directory.

var chroot: es_event_chroot_t

Properties of an event that indicates a change to a process’s root directory.

var exec: es_event_exec_t

Properties of an event that indicates the execution of a process.

var fork: es_event_fork_t

Properties of an event that indicates the forking of a process.

var proc_check: es_event_proc_check_t

Properties of an event that indicate the retrieval of process information.

var signal: es_event_signal_t

Properties of an event that indicates the sending of a signal to a process.

var exit: es_event_exit_t

Properties of an event that indicates a process exiting.

### Interprocess Events

var proc_suspend_resume: es_event_proc_suspend_resume_t

Properties of an event that indicates a call to suspend, resume, or shut down sockets for a process.

var trace: es_event_trace_t

Properties of an event that indicates an attempt by one process to attach to another.

var remote_thread_create: es_event_remote_thread_create_t

Properties of an event that indicates an attempt by one process to spawn a thread in another.

### Task Port Events

var get_task: es_event_get_task_t

Properties of an event that indicates the retrieval of a task’s control port.

var get_task_read: es_event_get_task_read_t

Properties of an event that indicates the retrieval of a task’s read port.

var get_task_inspect: es_event_get_task_inspect_t

Properties of an event that indicates the retrieval of a task’s inspect port.

var get_task_name: es_event_get_task_name_t

Properties of an event that indicates the retrieval of a task’s name port.

### User and Group ID Events

var setuid: es_event_setuid_t

Properties of an event that indicates a change to a process’s user ID.

var setgid: es_event_setgid_t

Properties of an event that indicates a change to a process’s group ID.

var seteuid: es_event_seteuid_t

Properties of an event that indicates a change to a process’s effective user ID.

var setegid: es_event_setegid_t

Properties of an event that indicates a change to a process’s effective group ID.

var setreuid: es_event_setreuid_t

Properties of an event that indicates a change to a process’s real and effective user IDs.

var setregid: es_event_setregid_t

Properties of an event that indicates a change to a process’s real and effective group IDs.

### Code Signing Events

var cs_invalidated: es_event_cs_invalidated_t

Properties of an event that indicates the invalidation of a process’s code signing status.

### Socket Events

var uipc_bind: es_event_uipc_bind_t

Properties of an event that indicates the binding of a socket to a path.

var uipc_connect: es_event_uipc_connect_t

Properties of an event that indicates the connection of a socket.

### Clock Events

var settime: es_event_settime_t

Properties of an event that indicates the modification of the system time.

### Kernel Events

var iokit_open: es_event_iokit_open_t

Properties of an event that indicates the opening of an IOKit device.

var kextload: es_event_kextload_t

Properties of an event that indicates the loading of a Kernel Extension (KEXT).

var kextunload: es_event_kextunload_t

Properties of an event that indicates the unloading of a Kernel Extension (KEXT).

### Pseudoterminal Events

var pty_close: es_event_pty_close_t

Properties of the event that indicates the closing of a pseudoterminal device.

var pty_grant: es_event_pty_grant_t

Properties of the event that indicates the granting of a pseudoterminal device to a user.

### Initializers

init(access: es_event_access_t)

init(authentication: UnsafeMutablePointer&lt;es_event_authentication_t>)

init(authorization_judgement: UnsafeMutablePointer&lt;es_event_authorization_judgement_t>)

init(authorization_petition: UnsafeMutablePointer&lt;es_event_authorization_petition_t>)

init(btm_launch_item_add: UnsafeMutablePointer&lt;es_event_btm_launch_item_add_t>)

init(btm_launch_item_remove: UnsafeMutablePointer&lt;es_event_btm_launch_item_remove_t>)

init(chdir: es_event_chdir_t)

init(chroot: es_event_chroot_t)

init(clone: es_event_clone_t)

init(close: es_event_close_t)

init(copyfile: es_event_copyfile_t)

init(create: es_event_create_t)

init(cs_invalidated: es_event_cs_invalidated_t)

init(deleteextattr: es_event_deleteextattr_t)

init(dup: es_event_dup_t)

init(exchangedata: es_event_exchangedata_t)

init(exec: es_event_exec_t)

init(exit: es_event_exit_t)

init(fcntl: es_event_fcntl_t)

init(file_provider_materialize: es_event_file_provider_materialize_t)

init(file_provider_update: es_event_file_provider_update_t)

init(fork: es_event_fork_t)

init(fsgetpath: es_event_fsgetpath_t)

init(gatekeeper_user_override: UnsafeMutablePointer&lt;es_event_gatekeeper_user_override_t>)

init(get_task: es_event_get_task_t)

init(get_task_inspect: es_event_get_task_inspect_t)

init(get_task_name: es_event_get_task_name_t)

init(get_task_read: es_event_get_task_read_t)

init(getattrlist: es_event_getattrlist_t)

init(getextattr: es_event_getextattr_t)

init(iokit_open: es_event_iokit_open_t)

init(kextload: es_event_kextload_t)

init(kextunload: es_event_kextunload_t)

init(link: es_event_link_t)

init(listextattr: es_event_listextattr_t)

init(login_login: UnsafeMutablePointer&lt;es_event_login_login_t>)

init(login_logout: UnsafeMutablePointer&lt;es_event_login_logout_t>)

init(lookup: es_event_lookup_t)

init(lw_session_lock: UnsafeMutablePointer&lt;es_event_lw_session_lock_t>)

init(lw_session_login: UnsafeMutablePointer&lt;es_event_lw_session_login_t>)

init(lw_session_logout: UnsafeMutablePointer&lt;es_event_lw_session_logout_t>)

init(lw_session_unlock: UnsafeMutablePointer&lt;es_event_lw_session_unlock_t>)

init(mmap: es_event_mmap_t)

init(mount: es_event_mount_t)

init(mprotect: es_event_mprotect_t)

init(od_attribute_set: UnsafeMutablePointer&lt;es_event_od_attribute_set_t>)

init(od_attribute_value_add: UnsafeMutablePointer&lt;es_event_od_attribute_value_add_t>)

init(od_attribute_value_remove: UnsafeMutablePointer&lt;es_event_od_attribute_value_remove_t>)

init(od_create_group: UnsafeMutablePointer&lt;es_event_od_create_group_t>)

init(od_create_user: UnsafeMutablePointer&lt;es_event_od_create_user_t>)

init(od_delete_group: UnsafeMutablePointer&lt;es_event_od_delete_group_t>)

init(od_delete_user: UnsafeMutablePointer&lt;es_event_od_delete_user_t>)

init(od_disable_user: UnsafeMutablePointer&lt;es_event_od_disable_user_t>)

init(od_enable_user: UnsafeMutablePointer&lt;es_event_od_enable_user_t>)

init(od_group_add: UnsafeMutablePointer&lt;es_event_od_group_add_t>)

init(od_group_remove: UnsafeMutablePointer&lt;es_event_od_group_remove_t>)

init(od_group_set: UnsafeMutablePointer&lt;es_event_od_group_set_t>)

init(od_modify_password: UnsafeMutablePointer&lt;es_event_od_modify_password_t>)

init(open: es_event_open_t)

init(openssh_login: UnsafeMutablePointer&lt;es_event_openssh_login_t>)

init(openssh_logout: UnsafeMutablePointer&lt;es_event_openssh_logout_t>)

init(proc_check: es_event_proc_check_t)

init(proc_suspend_resume: es_event_proc_suspend_resume_t)

init(profile_add: UnsafeMutablePointer&lt;es_event_profile_add_t>)

init(profile_remove: UnsafeMutablePointer&lt;es_event_profile_remove_t>)

init(pty_close: es_event_pty_close_t)

init(pty_grant: es_event_pty_grant_t)

init(readdir: es_event_readdir_t)

init(readlink: es_event_readlink_t)

init(remote_thread_create: es_event_remote_thread_create_t)

init(remount: es_event_remount_t)

init(rename: es_event_rename_t)

init(screensharing_attach: UnsafeMutablePointer&lt;es_event_screensharing_attach_t>)

init(screensharing_detach: UnsafeMutablePointer&lt;es_event_screensharing_detach_t>)

init(searchfs: es_event_searchfs_t)

init(setacl: es_event_setacl_t)

init(setattrlist: es_event_setattrlist_t)

init(setegid: es_event_setegid_t)

init(seteuid: es_event_seteuid_t)

init(setextattr: es_event_setextattr_t)

init(setflags: es_event_setflags_t)

init(setgid: es_event_setgid_t)

init(setmode: es_event_setmode_t)

init(setowner: es_event_setowner_t)

init(setregid: es_event_setregid_t)

init(setreuid: es_event_setreuid_t)

init(settime: es_event_settime_t)

init(setuid: es_event_setuid_t)

init(signal: es_event_signal_t)

init(stat: es_event_stat_t)

init(su: UnsafeMutablePointer&lt;es_event_su_t>)

init(sudo: UnsafeMutablePointer&lt;es_event_sudo_t>)

init(tcc_modify: UnsafeMutablePointer&lt;es_event_tcc_modify_t>)

init(trace: es_event_trace_t)

init(truncate: es_event_truncate_t)

init(uipc_bind: es_event_uipc_bind_t)

init(uipc_connect: es_event_uipc_connect_t)

init(unlink: es_event_unlink_t)

init(unmount: es_event_unmount_t)

init(utimes: es_event_utimes_t)

init(write: es_event_write_t)

init(xp_malware_detected: UnsafeMutablePointer&lt;es_event_xp_malware_detected_t>)

init(xp_malware_remediated: UnsafeMutablePointer&lt;es_event_xp_malware_remediated_t>)

init(xpc_connect: UnsafeMutablePointer&lt;es_event_xpc_connect_t>)

### Instance Properties

var authentication: UnsafeMutablePointer&lt;es_event_authentication_t>

var authorization_judgement: UnsafeMutablePointer&lt;es_event_authorization_judgement_t>

var authorization_petition: UnsafeMutablePointer&lt;es_event_authorization_petition_t>

var btm_launch_item_add: UnsafeMutablePointer&lt;es_event_btm_launch_item_add_t>

var btm_launch_item_remove: UnsafeMutablePointer&lt;es_event_btm_launch_item_remove_t>

var gatekeeper_user_override: UnsafeMutablePointer&lt;es_event_gatekeeper_user_override_t>

var login_login: UnsafeMutablePointer&lt;es_event_login_login_t>

var login_logout: UnsafeMutablePointer&lt;es_event_login_logout_t>

var lw_session_lock: UnsafeMutablePointer&lt;es_event_lw_session_lock_t>

var lw_session_login: UnsafeMutablePointer&lt;es_event_lw_session_login_t>

var lw_session_logout: UnsafeMutablePointer&lt;es_event_lw_session_logout_t>

var lw_session_unlock: UnsafeMutablePointer&lt;es_event_lw_session_unlock_t>

var od_attribute_set: UnsafeMutablePointer&lt;es_event_od_attribute_set_t>

var od_attribute_value_add: UnsafeMutablePointer&lt;es_event_od_attribute_value_add_t>

var od_attribute_value_remove: UnsafeMutablePointer&lt;es_event_od_attribute_value_remove_t>

var od_create_group: UnsafeMutablePointer&lt;es_event_od_create_group_t>

var od_create_user: UnsafeMutablePointer&lt;es_event_od_create_user_t>

var od_delete_group: UnsafeMutablePointer&lt;es_event_od_delete_group_t>

var od_delete_user: UnsafeMutablePointer&lt;es_event_od_delete_user_t>

var od_disable_user: UnsafeMutablePointer&lt;es_event_od_disable_user_t>

var od_enable_user: UnsafeMutablePointer&lt;es_event_od_enable_user_t>

var od_group_add: UnsafeMutablePointer&lt;es_event_od_group_add_t>

var od_group_remove: UnsafeMutablePointer&lt;es_event_od_group_remove_t>

var od_group_set: UnsafeMutablePointer&lt;es_event_od_group_set_t>

var od_modify_password: UnsafeMutablePointer&lt;es_event_od_modify_password_t>

var openssh_login: UnsafeMutablePointer&lt;es_event_openssh_login_t>

var openssh_logout: UnsafeMutablePointer&lt;es_event_openssh_logout_t>

var profile_add: UnsafeMutablePointer&lt;es_event_profile_add_t>

var profile_remove: UnsafeMutablePointer&lt;es_event_profile_remove_t>

var screensharing_attach: UnsafeMutablePointer&lt;es_event_screensharing_attach_t>

var screensharing_detach: UnsafeMutablePointer&lt;es_event_screensharing_detach_t>

var su: UnsafeMutablePointer&lt;es_event_su_t>

var sudo: UnsafeMutablePointer&lt;es_event_sudo_t>

var tcc_modify: UnsafeMutablePointer&lt;es_event_tcc_modify_t>

var xp_malware_detected: UnsafeMutablePointer&lt;es_event_xp_malware_detected_t>

var xp_malware_remediated: UnsafeMutablePointer&lt;es_event_xp_malware_remediated_t>

var xpc_connect: UnsafeMutablePointer&lt;es_event_xpc_connect_t>

## Relationships

### Conforms To

- Sendable

## See Also

### Identifying the Matched Event

var event: es_events_t

The event that triggered this message.

var event_type: es_event_type_t

The type of the message’s event.

struct es_event_type_t

A type used to identify a message’s event type and subscribe to events of that type.

