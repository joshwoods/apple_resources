

- Endpoint Security
-  ES_EVENT_TYPE_AUTH_SETACL 

Global Variable

# ES_EVENT_TYPE_AUTH_SETACL

An identifier for a process that requests permission from the operating system to set a file’s access control list.

Mac CatalystmacOS

``` source
var ES_EVENT_TYPE_AUTH_SETACL: es_event_type_t { get }
```

## Discussion

This identifier corresponds to the es_events_t union member setacl, which has the type es_event_setacl_t.

## See Also

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

