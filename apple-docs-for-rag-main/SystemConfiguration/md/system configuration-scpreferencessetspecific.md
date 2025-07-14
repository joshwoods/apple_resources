

- System Configuration
-  SCPreferencesSetSpecific 

API Collection

# SCPreferencesSetSpecific

## Overview

The functions in the `SCPreferencesSetSpecific` programming interface allow an application to set specific configuration information about the current system (for example, the computer or sharing name). Note that to access configuration preferences, you must first establish a preferences session using the SCPreferencesCreate(_:_:_:) function.

## Topics

### Setting Configuration Information

func SCPreferencesSetComputerName(SCPreferences, CFString?, CFStringEncoding) -> Bool

Sets the computer name preference to the specified name.

func SCPreferencesSetLocalHostName(SCPreferences, CFString?) -> Bool

Sets the local host name to the specified name.

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

SCPreferencesPath

SCSchemaDefinitions

System Configuration

SystemConfiguration Enumerations

SystemConfiguration Constants

SystemConfiguration Functions

SystemConfiguration Data Types

