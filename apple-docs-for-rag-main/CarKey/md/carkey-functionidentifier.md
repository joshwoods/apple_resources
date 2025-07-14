

- CarKey
-  FunctionIdentifier 

Structure

# FunctionIdentifier

A type that stores the designation code for one of your vehicle’s features.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.3+watchOS 9.0+

``` source
struct FunctionIdentifier
```

## Overview

A FunctionIdentifier type wraps a vehicle-specific code you define. This code — known as the function identifier — corresponds to a particular feature of your vehicle. For example, one function identifier might represent the vehicle’s door locks and another represent the vehicle’s window system. Use this type in conjunction with an ActionIdentifier type to specify the complete action you want to perform on a vehicle.

## Topics

### Creating a Function Identifier

init(rawValue: Int)

Creates and returns a new function identifier with the specified value.

init(Int)

Creates and returns a new function identifier with the specified value.

### Getting the Value

let rawValue: Int

The raw value that corresponds to the specific feature of your vehicle.

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

### Vehicle Actions

struct RemoteKeylessEntryAction

An automatically ending action that you want to perform on a vehicle.

struct RemoteKeylessEntryEnduringAction

An action with an optional stopping point that you want to perform on a vehicle.

Deprecated

struct ActionIdentifier

A type that stores the designation code for one of the actions that a vehicle feature supports.

