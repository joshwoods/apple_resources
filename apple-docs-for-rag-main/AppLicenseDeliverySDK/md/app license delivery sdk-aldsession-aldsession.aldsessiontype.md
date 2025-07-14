

- App License Delivery SDK
- ALDSession
-  ALDSession.ALDSessionType 

Enumeration

# ALDSession.ALDSessionType

The type of the license session created. A normalSession is used for a session created with a license request. A staticSession is used for session created without a license request

``` source
enum ALDSessionType
```

## Topics

### Enumeration Cases

case normalSession

case staticSession

case unknown

### Initializers

init?(rawValue: UInt32)

Creates a new instance with the specified raw value.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable

