

- System Configuration
-  SCDynamicStoreCallBack 

Type Alias

# SCDynamicStoreCallBack

Callback used when notification of changes made to the dynamic store is delivered.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias SCDynamicStoreCallBack = (SCDynamicStore, CFArray, UnsafeMutableRawPointer?) -> Void
```

## Topics

### Fields

store

The dynamic store session.

changedKeys

The list of changed keys.

info

A C pointer to a user-specified block of data.

## See Also

### Data Types

struct SCDynamicStoreContext

Structure containing user-specified data and callbacks for a dynamic store session.

class SCDynamicStore

The handle to an open dynamic store session with the system configuration daemon.

