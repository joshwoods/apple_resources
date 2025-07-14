

- Security
-  SecKeychainSettings 

Structure

# SecKeychainSettings

A structure that contains information about keychain settings.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct SecKeychainSettings
```

## Overview

This structure contains information about a keychain’s settings such as locking on sleep and the lock time interval. Use the SecKeychainSetSettings(_:_:) and SecKeychainCopySettings(_:_:) functions to set and copy a keychain’s settings.

## Topics

### Initializers

init()

Initializes a keychain settings structure with default values.

init(version: UInt32, lockOnSleep: DarwinBoolean, useLockInterval: DarwinBoolean, lockInterval: UInt32)

Initializes a keychain settings structures with the given values.

### Instance Properties

var lockInterval: UInt32

The number of seconds to wait before the keychain locks.

var lockOnSleep: DarwinBoolean

A Boolean value indicating whether the keychain locks when the system sleeps.

var useLockInterval: DarwinBoolean

A Boolean value indicating whether the keychain automatically locks after a certain period of time.

var version: UInt32

The keychain version.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

