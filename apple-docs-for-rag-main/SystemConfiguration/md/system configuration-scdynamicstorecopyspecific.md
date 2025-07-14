

- System Configuration
-  SCDynamicStoreCopySpecific 

API Collection

# SCDynamicStoreCopySpecific

## Overview

The functions of the `SCDynamicStoreCopySpecific` programming interface allow an application to determine specific configuration information about the current system (for example, the computer or sharing name or the currently logged-in user). Note that these functions follow Core Foundation function-name conventions. A function that has “Create” or “Copy” in its name returns a reference you must release with the CFRelease function.

## Topics

### Group

func SCDynamicStoreCopyComputerName(SCDynamicStore?, UnsafeMutablePointer&lt;CFStringEncoding>?) -> CFString?

Returns the current computer name.

func SCDynamicStoreCopyConsoleUser(SCDynamicStore?, UnsafeMutablePointer&lt;uid_t>?, UnsafeMutablePointer&lt;gid_t>?) -> CFString?

Returns information about the user currently logged into the system.

func SCDynamicStoreCopyLocalHostName(SCDynamicStore?) -> CFString?

Returns the current local host name.

func SCDynamicStoreCopyLocation(SCDynamicStore?) -> CFString?

Returns the current location identifier.

func SCDynamicStoreCopyProxies(SCDynamicStore?) -> CFDictionary?

Returns the key-value pairs that represent the current internet proxy settings.

## See Also

### Reference

SCDynamicStore

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

