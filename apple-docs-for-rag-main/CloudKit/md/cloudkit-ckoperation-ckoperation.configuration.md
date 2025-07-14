

- CloudKit
- CKOperation
-  CKOperation.Configuration 

Class

# CKOperation.Configuration

An object that describes how a CloudKit operation behaves.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class Configuration
```

## Overview

All of the properties in `CKOperationConfiguration` have a default value. When determining which properties to apply to a CloudKit operation, consult the operation’s configuration property, as well as the defaultConfiguration property of the group that the operation belongs to. These properties combine through the following rules:

| Group default configuration value | Operation configuration value | Value applied to operation |
|----|----|----|
| default value | default value | default value |
| default value | explicit value | operation.configuration explicit value |
| explicit value | default value | group.defaultConfiguration explicit value |
| explicit value | explicit value | operation.configuration explicit value |

## Topics

### Preparing a Configuration

var allowsCellularAccess: Bool

A Boolean value that indicates whether operations that use this configuration can send data over the cellular network.

var container: CKContainer?

The configuration’s container.

var isLongLived: Bool

A Boolean value that indicates whether the operations that use this configuration are long-lived.

var qualityOfService: QualityOfService

The priority that the system uses when it allocates resources to the operations that use this configuration.

var timeoutIntervalForRequest: TimeInterval

The maximum amount of time that a request can take.

var timeoutIntervalForResource: TimeInterval

The maximum amount of time that a resource request can take.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Managing the Operation’s Configuration

var configuration: CKOperation.Configuration!

The operation’s configuration.

var group: CKOperationGroup?

The operation’s group.

var longLivedOperationWasPersistedBlock: (() -> Void)?

The closure to execute when the server begins to store callbacks for the long-lived operation.

