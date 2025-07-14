

- Endpoint Security
- es_events_t
-  signal 

Instance Property

# signal

Properties of an event that indicates the sending of a signal to a process.

Mac CatalystmacOS

``` source
var signal: es_event_signal_t { get set }
```

## Discussion

Endpoint Security doesn’t fire this event if a process sends a signal to itself.

## See Also

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

var exit: es_event_exit_t

Properties of an event that indicates a process exiting.

