

- SwiftUI
-  FocusedObject 

Structure

# FocusedObject

A property wrapper type for an observable object supplied by the focused view or one of its ancestors.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @frozen @propertyWrapper @preconcurrency
struct FocusedObject where ObjectType : ObservableObject
```

## Overview

Focused objects invalidate the current view whenever the observable object changes. If multiple views publish a focused object using the same key, the wrapped property will reflect the object that’s closest to the focused view.

## Topics

### Creating the focused object

init()

Creates a focused object.

### Getting the value

var projectedValue: FocusedObject&lt;ObjectType>.Wrapper?

A projection of the focused object that creates bindings to its properties using dynamic member lookup.

var wrappedValue: ObjectType?

The underlying value referenced by the focused object.

struct Wrapper

A wrapper around the underlying focused object that can create bindings to its properties using dynamic member lookup.

## Relationships

### Conforms To

- DynamicProperty

## See Also

### Exposing reference types to focused views

func focusedObject(_:)

Creates a new view that exposes the provided object to other views whose whose state depends on the focused view hierarchy.

func focusedSceneObject(_:)

Creates a new view that exposes the provided object to other views whose whose state depends on the active scene.

