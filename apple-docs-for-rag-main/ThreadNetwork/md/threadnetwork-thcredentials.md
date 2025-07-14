

- ThreadNetwork
-  THCredentials 

Class

# THCredentials

A class that contains credentials for a Thread network.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 13.0+visionOS 1.0+

``` source
class THCredentials
```

## Overview

A Thread network defines parameters that all connected devices use. THCredentials provides these parameters.

## Topics

### Getting the Thread Parameters

var activeOperationalDataSet: Data?

The essential operational parameters for the Thread network.

var borderAgentID: Data?

The identifer of an active Thread network Border Agent.

var channel: UInt8

The Thread network radio channel.

var extendedPANID: Data?

The Thread network extended PAN identifier.

var networkKey: Data?

The Thread network key.

var networkName: String?

The Thread network name.

var panID: Data?

The Thead network PAN identifier.

var pskc: Data?

The Thread network pre-shared key for the Commissioner.

### Getting the Framework Parameters

var creationDate: Date?

The date and time that the framework stored the credential in the database.

var lastModificationDate: Date?

The date and time that the framework updated the credential in the database.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Managing clients and sharing credentials

com.apple.developer.networking.manage-thread-network-credentials

A Boolean value that indicates whether the app can use ThreadNetwork.

class THClient

A class that supports safely sharing Thread credentials between multiple clients.

