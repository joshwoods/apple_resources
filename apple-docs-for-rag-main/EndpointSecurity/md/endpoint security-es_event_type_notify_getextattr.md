

- Endpoint Security
-  ES_EVENT_TYPE_NOTIFY_GETEXTATTR 

Global Variable

# ES_EVENT_TYPE_NOTIFY_GETEXTATTR

An identifier for a process that notifies endpoint security that it is retrieving an extended attribute from a file.

Mac CatalystmacOS

``` source
var ES_EVENT_TYPE_NOTIFY_GETEXTATTR: es_event_type_t { get }
```

## Discussion

This identifier corresponds to the es_events_t union member getextattr, which has the type es_event_getextattr_t.

## See Also

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

