

- System Configuration
-  SCPreferencesPath 

API Collection

# SCPreferencesPath

## Overview

The `SCPreferencesPath` programming interface allows an application to load and store XML configuration data in a controlled manner and provide the necessary notifications to other applications that need to be aware of configuration changes.

The functions in this programming interface view the data as a collection of dictionaries of key-value pairs and an associated path name. The root path (”/”) identifies the top-level dictionary. Additional path components specify the keys for subdictionaries.

For example, the following dictionary can be accessed via two paths. The root path (”/”) returns a dictionary with all keys and values. The path “/path1” returns only the dictionary with the “key3” and “key4” properties.

```
```

Each dictionary can also include the `kSCResvLink` (”\_\_LINK\_\_”) key. The value associated with this key is interpreted as a link to another path. If this key is present, a call to the SCPreferencesPathGetValue(_:_:) function returns the dictionary specified by the link.

## Topics

### Creating a New Path

func SCPreferencesPathCreateUniqueChild(SCPreferences, CFString) -> CFString?

Creates a new path component rooted at the specified path in the dictionary hierarchy.

### Associating Information with a Path

func SCPreferencesPathSetValue(SCPreferences, CFString, CFDictionary) -> Bool

Associates the specified dictionary with the specified path.

func SCPreferencesPathSetLink(SCPreferences, CFString, CFString) -> Bool

Associates a link to a second dictionary at the specified path.

### Getting or Removing Information Associated with a Path

func SCPreferencesPathGetValue(SCPreferences, CFString) -> CFDictionary?

Returns the dictionary associated with the specified path.

func SCPreferencesPathGetLink(SCPreferences, CFString) -> CFString?

Returns the link associated with the specified path.

func SCPreferencesPathRemoveValue(SCPreferences, CFString) -> Bool

Removes the data associated with the specified path.

## See Also

### Reference

SCDynamicStore

SCDynamicStoreCopySpecific

SCDynamicStoreKey

SCNetwork

SCNetworkConfiguration

SCNetworkConnection

SCNetworkReachability

SCPreferences

SCPreferencesSetSpecific

SCSchemaDefinitions

System Configuration

SystemConfiguration Enumerations

SystemConfiguration Constants

SystemConfiguration Functions

SystemConfiguration Data Types

