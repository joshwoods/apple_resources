

- SwiftUI
-  EnvironmentObject 

Structure

# EnvironmentObject

A property wrapper type for an observable object that a parent or ancestor view supplies.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @frozen @propertyWrapper @preconcurrency
struct EnvironmentObject where ObjectType : ObservableObject
```

## Overview

An environment object invalidates the current view whenever the observable object that conforms to ObservableObject changes. If you declare a property as an environment object, be sure to set a corresponding model object on an ancestor view by calling its environmentObject(_:) modifier.

Note

If your observable object conforms to the Observable protocol, use Environment instead of `EnvironmentObject` and set the model object in an ancestor view by calling its environment(_:) or environment(_:_:) modifiers.

## Topics

### Creating an environment object

init()

Creates an environment object.

### Getting the value

var wrappedValue: ObjectType

The underlying value referenced by the environment object.

var projectedValue: EnvironmentObject&lt;ObjectType>.Wrapper

A projection of the environment object that creates bindings to its properties using dynamic member lookup.

struct Wrapper

A wrapper of the underlying environment object that can create bindings to its properties using dynamic member lookup.

## Relationships

### Conforms To

- DynamicProperty
- Sendable

## See Also

### Distributing model data throughout your app

func environmentObject&lt;T>(T) -> some View

Supplies an observable object to a view’s hierarchy.

func environmentObject&lt;T>(T) -> some Scene

Supplies an `ObservableObject` to a view subhierarchy.

