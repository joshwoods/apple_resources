

- ContactProvider
-  ContactItem 

Enumeration

# ContactItem

An item in the contact database.

iOS 18.0+iPadOS 18.0+

``` source
enum ContactItem
```

## Overview

Your app creates instances of this type in your implementations of ContactItemEnumerator, delivering arrays of contact items to ContactItemContentObserver and ContactItemChangeObserver instances.

## Topics

### Handling item type

case contact(CNMutableContact, ContactItem.Identifier)

An item that represents a person or organization.

### Identifying the item

struct Identifier

The app’s identifier for an item in the contact database.

### Hashing

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

### Comparing contact items

static func == (ContactItem, ContactItem) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Providing contacts

protocol ContactItemEnumerating

A protocol to provide enumerators for collections of contact items.

protocol ContactItemEnumerator

A protocol to provide enumerations of all contact items and changed contact items.

