

- Security
-  SecKeychainEvent 

Enumeration

# SecKeychainEvent

The list of keychain events that can trigger a callback.

Mac Catalyst 13.0+macOS 10.0+

``` source
enum SecKeychainEvent
```

## Overview

Keychain Services includes one of these events in the callback you register with SecKeychainAddCallback(_:_:_:), using the function signature defined by SecKeychainCallback, to indicate what event triggered the callback.

## Topics

### Constants

case lockEvent

Indicates a keychain was locked.

case unlockEvent

Indicates a keychain was successfully unlocked.

case addEvent

Indicates an item was added to a keychain.

case deleteEvent

Indicates an item was deleted from a keychain.

case updateEvent

Indicates a keychain item was updated.

case passwordChangedEvent

Indicates the keychain password was changed.

case defaultChangedEvent

Indicates that a different keychain was specified as the default.

case dataAccessEvent

Indicates a process has accessed a keychain item’s data.

Deprecated

case keychainListChangedEvent

Indicates the list of keychains has changed.

case trustSettingsChangedEvent

Indicates trust settings have changed.

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

