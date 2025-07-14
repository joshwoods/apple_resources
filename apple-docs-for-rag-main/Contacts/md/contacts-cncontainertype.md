

- Contacts
-  CNContainerType 

Enumeration

# CNContainerType

The container may be local on the device or associated with a server account that has contacts.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
enum CNContainerType
```

## Topics

### Constants

case local

A container for contacts only stored locally on the device.

case exchange

A container for contacts stored in an Exchange folder from an Exchange server.

case cardDAV

A container for contacts stored in an CardDAV server, such as iCloud.

case unassigned

A container where the system hasn’t assigned the container type.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the Container Information

var name: String

The name of the container.

var identifier: String

The unique identifier for a contacts container on the device.

var type: CNContainerType

The type of the container.

