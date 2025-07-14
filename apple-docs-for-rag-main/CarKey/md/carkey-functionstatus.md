

- CarKey
-  FunctionStatus 

Structure

# FunctionStatus

A value that the vehicle can return to indicate the status of a particular vehicle feature.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.3+watchOS 9.0+

``` source
struct FunctionStatus
```

## Overview

A FunctionStatus type wraps the custom code that the vehicle returns. You define the status codes and their meanings for your vehicle’s features. For example, you might define status codes to represent the locked, unlocked, and unknown states of your vehicle’s door-locking system.

## Topics

### Creating a Function Status Type

init(rawValue: Int)

Creates and returns a new function status with the specified value.

init(Int)

Creates and returns a new function status with the specified value.

### Getting the Value

let rawValue: Int

The raw value that corresponds to the feature-specific status.

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

### Getting the Vehicle’s Supported Functions

var supportedFunctions: [FunctionIdentifier]

An array of function identifiers that indicates the features the vehicle supports, populated only after the first BLE connection with the vehicle.

func status(for: FunctionIdentifier) throws -> FunctionStatus?

Returns the current status of the specified vehicle function.

