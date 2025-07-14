

- Swift
-  ObjectIdentifier 

Structure

# ObjectIdentifier

A unique identifier for a class instance or metatype.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct ObjectIdentifier
```

## Overview

This unique identifier is only valid for comparisons during the lifetime of the instance.

In Swift, only class instances and metatypes have unique identities. There is no notion of identity for structs, enums, functions, or tuples.

## Topics

### Initializers

init(AnyObject)

Creates an instance that uniquely identifies the given class instance.

init(any Any.Type)

Creates an instance that uniquely identifies the given metatype.

### Default Implementations

AtomicOptionalRepresentable Implementations

AtomicRepresentable Implementations

Comparable Implementations

CustomDebugStringConvertible Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- AtomicOptionalRepresentable
- AtomicRepresentable
- BitwiseCopyable
- Comparable
- Copyable
- CustomDebugStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Querying Runtime Values

struct Mirror

A representation of the substructure and display style of an instance of any type.

func type&lt;T, Metatype>(of: T) -> Metatype

Returns the dynamic type of a value.

func == ((any Any.Type)?, (any Any.Type)?) -> Bool

Returns a Boolean value indicating whether two types are identical.

func != ((any Any.Type)?, (any Any.Type)?) -> Bool

Returns a Boolean value indicating whether two types are not identical.

