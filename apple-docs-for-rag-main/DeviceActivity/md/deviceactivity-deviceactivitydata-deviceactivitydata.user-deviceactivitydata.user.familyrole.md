

- DeviceActivity
- DeviceActivityData
- DeviceActivityData.User
-  DeviceActivityData.User.FamilyRole 

Enumeration

# DeviceActivityData.User.FamilyRole

A type describing the user’s role in their iCloud family.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
enum FamilyRole
```

## Overview

If the user is not signed into an iCloud account or in an iCloud family, then they are an `individual`.

## Topics

### Enumeration Cases

case child

A child that is being managed by a parent or guardian in their iCloud family.

case individual

An individual that has authorized your app with `FamilyControls`.

### Initializers

init?(rawValue: Int)

Creates a new instance with the specified raw value.

### Instance Properties

var rawValue: Int

The corresponding value of the raw type.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable

