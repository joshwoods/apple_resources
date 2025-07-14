

- Security
-  SecKeychainEventMask 

Structure

# SecKeychainEventMask

Bit masks corresponding to the events that can trigger a keychain callback.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct SecKeychainEventMask
```

## Overview

Bitwise `OR` one or more of these masks together to provide the `eventMask` input to the SecKeychainAddCallback(_:_:_:) function to indicate what event or events should trigger your callback.

## Topics

### Initializers

init(rawValue: UInt32)

Initializes an event mask value.

### Constants

static var lockEventMask: SecKeychainEventMask

If the bit specified by this mask is set, your callback function is invoked when a keychain is locked.

static var unlockEventMask: SecKeychainEventMask

If the bit specified by this mask is set, your callback function is invoked when a keychain is unlocked.

static var addEventMask: SecKeychainEventMask

If the bit specified by this mask is set, your callback function is invoked when an item is added to a keychain.

static var deleteEventMask: SecKeychainEventMask

If the bit specified by this mask is set, your callback function is invoked when an item is deleted from a keychain.

static var updateEventMask: SecKeychainEventMask

If the bit specified by this mask is set, your callback function is invoked when a keychain item is updated.

static var passwordChangedEventMask: SecKeychainEventMask

If the bit specified by this mask is set, your callback function is invoked when the keychain password is changed.

static var defaultChangedEventMask: SecKeychainEventMask

If the bit specified by this mask is set, your callback function is invoked when a different keychain is specified as the default.

static var dataAccessEventMask: SecKeychainEventMask

If the bit specified by this mask is set, your callback function is invoked when a process accesses a keychain item’s data.

Deprecated

static var keychainListChangedMask: SecKeychainEventMask

If the bit specified by this mask is set, your callback function is invoked when a keychain list is changed.

static var trustSettingsChangedEventMask: SecKeychainEventMask

If the bit specified by this mask is set, your callback function is invoked when there is a change in certificate trust settings.

static var everyEventMask: SecKeychainEventMask

If all the bits are set, your callback function is invoked whenever any event occurs.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

