

- DeviceActivity
- DeviceActivityEvent
-  DeviceActivityEvent.Name 

Structure

# DeviceActivityEvent.Name

The unique name of an event.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
struct Name
```

## Overview

`DeviceActivityEvent.Name` allows applications to associate an event with some of their own data.

## Topics

### Accessing the Raw Value

init(rawValue: String)

Creates a new instance with the specified raw value.

init(String)

Creates a new instance with the specified raw value.

var rawValue: String

The corresponding value of the raw type.

### Identifying and Comparing Errors

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two values aren’t equal.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable

## See Also

### Creating an Event

init(applications: Set&lt;ApplicationToken>, categories: Set&lt;ActivityCategoryToken>, webDomains: Set&lt;WebDomainToken>, threshold: DateComponents)

Creates a new event.

var includesAllActivity: Bool

A Boolean value that indicates whether the event includes all applications, categories, and web domains.

