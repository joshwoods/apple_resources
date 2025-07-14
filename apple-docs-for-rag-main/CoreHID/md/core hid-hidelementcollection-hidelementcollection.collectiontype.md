

- Core HID
- HIDElementCollection
-  HIDElementCollection.CollectionType 

Enumeration

# HIDElementCollection.CollectionType

Types of HIDElementCollections.

macOS 15.0+

``` source
enum CollectionType
```

## Overview

Collection types are a defined part of the HID specification that define how a collection is intended to be used.

See the HID specification for more details: https://www.usb.org/hid.

## Topics

### Operators

static func == (HIDElementCollection.CollectionType, HIDElementCollection.CollectionType) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case application

case logical

case namedArray

case physical

case report

case usageModifier

case usageSwitch

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

