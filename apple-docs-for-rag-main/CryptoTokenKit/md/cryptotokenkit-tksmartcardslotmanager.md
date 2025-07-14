

- CryptoTokenKit
-  TKSmartCardSlotManager 

Class

# TKSmartCardSlotManager

An interface to all available smart card reader slots.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class TKSmartCardSlotManager
```

## Overview

Get a list of all known smart card reader slots in the system using the slotNames property, and access individual slots by name using the getSlot(withName:reply:) method.

Important

The com.apple.security.smartcard entitlement is required in order to use `TKSmartCardSlotManager`.

## Topics

### Creating a Card Slot Manager

class var `default`: TKSmartCardSlotManager?

The shared singleton Smart Card reader slot manager.

### Accessing Smart Card Slots

var slotNames: [String]

A list of identifiers for all the Smart Card reader slots available to the system.

func getSlot(withName: String, reply: (TKSmartCardSlot?) -> Void)

Asynchronously calls a block with a Smart Card reader slot for a specified name.

func slotNamed(String) -> TKSmartCardSlot?

Returns the Smart Card slot with a given name.

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

## See Also

### Smart Cards

Using Cryptographic Assets Stored on a Smart Card

Access certificates, keys, and identities stored on a smart card as if they were part of the keychain.

class TKSmartCardSlot

A single smart card reader slot in the system.

class TKSmartCard

A representation of a smart card.

