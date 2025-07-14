

- System Configuration
-  SCNetwork 

API Collection

# SCNetwork

## Overview

The `SCNetwork` programming interface contains functions an application can use to determine whether that application can reach a remote host and to notify the system of configuration changes.

A remote host is considered reachable when a data packet, sent by an application into the network stack, can leave the local computer. Note that reachability does not guarantee that the data packet will actually be received by the host.

## Topics

### Constants

typealias SCNetworkConnectionFlags

Flags that indicate whether the specified network node name or address is reachable, whether a connection is required, and whether some user intervention may be required when establishing a connection.

## See Also

### Reference

SCDynamicStore

SCDynamicStoreCopySpecific

SCDynamicStoreKey

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

