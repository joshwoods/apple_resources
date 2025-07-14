

- CarKey
-  ActionIdentifier 

Structure

# ActionIdentifier

A type that stores the designation code for one of the actions that a vehicle feature supports.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.3+watchOS 9.0+

``` source
struct ActionIdentifier
```

## Overview

An ActionIdentifier type wraps a vehicle-specific code you define. This code — known as the action identifier — corresponds to an action your vehicle can take for a particular feature. For example, you might define actions to lock or unlock the vehicle’s doors. Use this type in conjunction with a specific FunctionIdentifier type to specify the complete action you want to perform on a vehicle.

## Topics

### Creating the Action Identifier

init(rawValue: Int)

Creates and returns a new action identifier with the specified value.

init(Int)

Creates and returns a new action identifier with the specified value.

### Getting the Value

let rawValue: Int

The raw value that corresponds to the feature-specific action.

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

struct FunctionIdentifier

A type that stores the designation code for one of your vehicle’s features.

