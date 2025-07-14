

- Foundation
-  NSKeyValueChange 

Enumeration

# NSKeyValueChange

The kinds of changes that can be observed.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum NSKeyValueChange
```

## Overview

These constants are returned as the value for a kindKey key in the change dictionary passed to observeValue(forKeyPath:of:change:context:) indicating the type of change made.

## Topics

### Constants

case setting

Indicates that the value of the observed key path was set to a new value. This change can occur when observing an attribute of an object, as well as properties that specify to-one and to-many relationships.

case insertion

Indicates that an object has been inserted into the to-many relationship that is being observed.

case removal

Indicates that an object has been removed from the to-many relationship that is being observed.

case replacement

Indicates that an object has been replaced in the to-many relationship that is being observed.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Enumerations

enum NSGrammaticalCase

enum NSGrammaticalDefiniteness

enum NSGrammaticalDetermination

enum NSGrammaticalPerson

enum NSGrammaticalPronounType

struct NSKeyValueObservingOptions

The values that can be returned in a change dictionary.

enum NSKeyValueSetMutationKind

