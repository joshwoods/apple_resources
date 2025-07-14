

- Security
-  AuthorizationItemSet 

Structure

# AuthorizationItemSet

A structure containing a set of authorization items.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct AuthorizationItemSet
```

## Overview

Because it is actually a set, the list of items should not contain any duplicates.

## Topics

### Initializers

init()

Initializes an authorization item set.

init(count: UInt32, items: UnsafeMutablePointer&lt;AuthorizationItem>?)

Initializes an authorization item set with the given items.

### Instance Properties

var count: UInt32

The number of elements in the `items` array.

var items: UnsafeMutablePointer&lt;AuthorizationItem>?

A pointer to an array of authorization items.

## Relationships

### Conforms To

- BitwiseCopyable

