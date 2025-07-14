

- ContactProvider
-  ContactItemEnumerating 

Protocol

# ContactItemEnumerating

A protocol to provide enumerators for collections of contact items.

iOS 18.0+iPadOS 18.0+

``` source
protocol ContactItemEnumerating
```

## Overview

You typically implement this protocol in your app extension, since ContactProviderExtension inherits this protocol.

## Topics

### Providing an enumeration

func enumerator(for: ContactItem.Identifier) -> any ContactItemEnumerator

Provide an enumerator for the contact items collection.

**Required**

struct Identifier

The app’s identifier for an item in the contact database.

protocol ContactItemEnumerator

A protocol to provide enumerations of all contact items and changed contact items.

## Relationships

### Inherited By

- ContactProviderExtension

## See Also

### Providing contacts

enum ContactItem

An item in the contact database.

protocol ContactItemEnumerator

A protocol to provide enumerations of all contact items and changed contact items.

