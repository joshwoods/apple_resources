

- SwiftUI
-  FocusedBinding 

Structure

# FocusedBinding

A convenience property wrapper for observing and automatically unwrapping state bindings from the focused view or one of its ancestors.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@propertyWrapper
struct FocusedBinding
```

## Overview

If multiple views publish bindings using the same key, the wrapped property will reflect the value of the binding from the view closest to focus.

## Topics

### Creating the binding

init(KeyPath&lt;FocusedValues, Binding&lt;Value>?>)

A new property wrapper for the given key path.

### Getting the value

var projectedValue: Binding&lt;Value?>

A binding to the optional value.

var wrappedValue: Value?

The unwrapped value for the focus key given the current scope and state of the focused view hierarchy.

## Relationships

### Conforms To

- DynamicProperty

## See Also

### Managing focus state

func focused&lt;Value>(FocusState&lt;Value>.Binding, equals: Value) -> some View

Modifies this view by binding its focus state to the given state value.

func focused(FocusState&lt;Bool>.Binding) -> some View

Modifies this view by binding its focus state to the given Boolean state value.

var isFocused: Bool

Returns whether the nearest focusable ancestor has focus.

struct FocusState

A property wrapper type that can read and write a value that SwiftUI updates as the placement of focus within the scene changes.

struct FocusedValue

A property wrapper for observing values from the focused view or one of its ancestors.

macro Entry()

Creates an environment values, transaction, container values, or focused values entry.

protocol FocusedValueKey

A protocol for identifier types used when publishing and observing focused values.

func searchFocused(FocusState&lt;Bool>.Binding) -> some View

Modifies this view by binding the focus state of the search field associated with the nearest searchable modifier to the given Boolean value.

func searchFocused&lt;V>(FocusState&lt;V>.Binding, equals: V) -> some View

Modifies this view by binding the focus state of the search field associated with the nearest searchable modifier to the given value.

