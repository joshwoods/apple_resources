

- Endpoint Security
- es_events_t
-  trace 

Instance Property

# trace

Properties of an event that indicates an attempt by one process to attach to another.

Mac CatalystmacOS

``` source
var trace: es_event_trace_t { get set }
```

## See Also

### Interprocess Events

var proc_suspend_resume: es_event_proc_suspend_resume_t

Properties of an event that indicates a call to suspend, resume, or shut down sockets for a process.

var remote_thread_create: es_event_remote_thread_create_t

Properties of an event that indicates an attempt by one process to spawn a thread in another.

