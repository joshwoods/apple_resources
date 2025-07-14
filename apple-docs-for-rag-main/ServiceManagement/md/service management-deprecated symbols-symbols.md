

- Service Management
-  Deprecated Symbols 

API Collection

# Deprecated Symbols

## Topics

### Deprecated Constants

let kSMErrorDomainFramework: CFString!

A Service Management error domain.

Deprecated

let kSMErrorDomainIPC: CFString!

A Service Management IPC error domain.

Deprecated

let kSMErrorDomainLaunchd: CFString!

A Service Management `launchd` error domain.

Deprecated

### Deprecated Functions

func SMCopyAllJobDictionaries(CFString!) -> Unmanaged&lt;CFArray>!

Copies the job description dictionaries for all jobs in the specified domain.

Deprecated

func SMJobCopyDictionary(CFString!, CFString) -> Unmanaged&lt;CFDictionary>!

Copies the job description dictionary for the specified job label.

Deprecated

func SMJobRemove(CFString!, CFString, UnsafeMutableRawPointer!, Bool, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Removes the job with the specified label from the specified domain.

Deprecated

func SMJobSubmit(CFString!, CFDictionary, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Submits the specified job to the specified domain.

Deprecated

### Deprecated Property List Keys

kSMInfoKeyAuthorizedClients

The authorized clients property list key.

kSMInfoKeyPrivilegedExecutables

The privileged executables property list key.

