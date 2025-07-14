

- System Configuration
-  SCDynamicStore 

API Collection

# SCDynamicStore

## Overview

The `SCDynamicStore` programming interface provides access to the key-value pairs in the dynamic store of a running system. The dynamic store contains, among other items, a copy of the configuration settings for the currently active set (which is sometimes refered to as the location) and information about the current network state.

The functions in the `SCDynamicStore` programming interface allow you to find key-value pairs, add or remove key-value pairs, add or change values, and request notifications. Note that these functions follow Core Foundation function-name conventions. A function that has “Create” or “Copy” in its name returns a reference you must release with the CFRelease function.

To use these functions, you must first establish a dynamic store session using the SCDynamicStoreCreate(_:_:_:_:) function. When you are finished with the session, use `CFRelease` to close it.

## Topics

### Creating a Dynamic Store Session

func SCDynamicStoreCreateWithOptions(CFAllocator?, CFString, CFDictionary?, SCDynamicStoreCallBack?, UnsafeMutablePointer&lt;SCDynamicStoreContext>?) -> SCDynamicStore?

Creates a new session used to interact with the dynamic store maintained by the System Configuration server.

func SCDynamicStoreCreate(CFAllocator?, CFString, SCDynamicStoreCallBack?, UnsafeMutablePointer&lt;SCDynamicStoreContext>?) -> SCDynamicStore?

Creates a new session used to interact with the dynamic store maintained by the System Configuration server.

### Adding or Updating Keys and Values

func SCDynamicStoreAddTemporaryValue(SCDynamicStore, CFString, CFPropertyList) -> Bool

Temporarily adds the specified key-value pair to the dynamic store, if no such key already exists.

func SCDynamicStoreAddValue(SCDynamicStore?, CFString, CFPropertyList) -> Bool

Adds the specified key-value pair to the dynamic store, if no such key already exists.

func SCDynamicStoreSetMultiple(SCDynamicStore?, CFDictionary?, CFArray?, CFArray?) -> Bool

Updates multiple values in the dynamic store.

func SCDynamicStoreSetValue(SCDynamicStore?, CFString, CFPropertyList) -> Bool

Adds or replaces a value in the dynamic store for the specified key.

### Getting Keys and Values

func SCDynamicStoreCopyKeyList(SCDynamicStore?, CFString) -> CFArray?

Returns the keys that represent the current dynamic store entries that match the specified pattern.

func SCDynamicStoreCopyMultiple(SCDynamicStore?, CFArray?, CFArray?) -> CFDictionary?

Returns the key-value pairs that match the specified keys and key patterns.

func SCDynamicStoreCopyNotifiedKeys(SCDynamicStore) -> CFArray?

Returns the keys that have changed since the last call to this function.

func SCDynamicStoreCopyValue(SCDynamicStore?, CFString) -> CFPropertyList?

Returns the value associated with the specified key.

### Monitoring Keys and Values

func SCDynamicStoreNotifyValue(SCDynamicStore?, CFString) -> Bool

Causes a notification to be delivered for the specified key in the dynamic store.

func SCDynamicStoreSetNotificationKeys(SCDynamicStore, CFArray?, CFArray?) -> Bool

Specifies a set of keys and key patterns that should be monitored for changes.

func SCDynamicStoreSetDispatchQueue(SCDynamicStore, dispatch_queue_t?) -> Bool

Initiates notifications for the notification keys, using the specified dispatch queue for the callback.

### Removing Keys and Values

func SCDynamicStoreRemoveValue(SCDynamicStore?, CFString) -> Bool

Removes the value of the specified key from the dynamic store.

### Creating a Run Loop Source

func SCDynamicStoreCreateRunLoopSource(CFAllocator?, SCDynamicStore, CFIndex) -> CFRunLoopSource?

Creates a run loop source object that can be added to the application’s run loop.

### Getting Information About the Dynamic Store

func SCDynamicStoreGetTypeID() -> CFTypeID

Returns the type identifier of all `SCDynamicStore` instances.

### Data Types

typealias SCDynamicStoreCallBack

Callback used when notification of changes made to the dynamic store is delivered.

struct SCDynamicStoreContext

Structure containing user-specified data and callbacks for a dynamic store session.

class SCDynamicStore

The handle to an open dynamic store session with the system configuration daemon.

### Constants

Dynamic Store Options Keys

Keys that indicate the options for a dynamic store session.

## See Also

### Reference

SCDynamicStoreCopySpecific

SCDynamicStoreKey

SCNetwork

SCNetworkConfiguration

SCNetworkConnection

SCNetworkReachability

SCPreferences

SCPreferencesPath

SCPreferencesSetSpecific

SCSchemaDefinitions

System Configuration

SystemConfiguration Enumerations

SystemConfiguration Constants

SystemConfiguration Functions

SystemConfiguration Data Types

