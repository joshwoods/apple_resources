

- ContactProvider
-  ContactItemEnumerator 

Protocol

# ContactItemEnumerator

A protocol to provide enumerations of all contact items and changed contact items.

iOS 18.0+iPadOS 18.0+

``` source
protocol ContactItemEnumerator
```

## Overview

Implement this protocol to fetch contact items from your data store in a consistent, predictable order when the system requests contact item enumeration. The ContactItemEnumerating protocol, typically implemented by the app extension, returns an instance of this type when the system requests contacts.

The enumerator has two main methods to implement:

- enumerateContent(in:for:) – Enumerates all of your contacts that you want to provide to the system-wide Contacts ecosystem, sending arrays of ContactItem instances to a ContactItemContentObserver.

- enumerateChanges(startingAt:for:) – Enumerates changed contacts, sending updates and deletions to a ContactItemChangeObserver, as arrays of ContactItem and ContactItem.Identifier instances, respectively.

The following `RootContainerEnumerator` outlines how to implement a `ContactItemEnumerator`. The listing shows `TODO` in places where the implementation depends on the specifics of your app’s data store.

```
```

## Topics

### Enumerating contact items

func enumerateContent(in: ContactItemPage, for: any ContactItemContentObserver) async

Enumerates all items, batched in pages.

**Required**

struct ContactItemPage

A fixed offset into enumerating all contact items.

protocol ContactItemContentObserver

A protocol that defines a system observer that receives a resumable enumeration of all items.

### Enumerating item changes

func enumerateChanges(startingAt: ContactItemSyncAnchor, for: any ContactItemChangeObserver) async

Enumerates items changed since the last sync.

**Required**

struct ContactItemSyncAnchor

A snapshot point into enumerating changed contact items.

protocol ContactItemChangeObserver

A protocol that defines a system observer that receives a resumable enumeration of changed contact items.

### Managing enumerator life cycle

func invalidate() async

Invalidates the enumerator.

**Required**

## See Also

### Providing contacts

enum ContactItem

An item in the contact database.

protocol ContactItemEnumerating

A protocol to provide enumerators for collections of contact items.

