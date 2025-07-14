

- SwiftUI
-  Binding 

Structure

# Binding

A property wrapper type that can read and write a value owned by a source of truth.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen @propertyWrapper @dynamicMemberLookup
struct Binding
```

## Mentioned in 

Performing a search operation

Managing search interface activation

Adding a search interface to your app

Managing user interface state

## Overview

Use a binding to create a two-way connection between a property that stores data, and a view that displays and changes the data. A binding connects a property to a source of truth stored elsewhere, instead of storing data directly. For example, a button that toggles between play and pause can create a binding to a property of its parent view using the `Binding` property wrapper.

```
struct PlayButton: View {
    @Binding var isPlaying: Bool

    var body: some View {
        Button(isPlaying ? "Pause" : "Play") {
            isPlaying.toggle()
        }
    }
}
```

The parent view declares a property to hold the playing state, using the State property wrapper to indicate that this property is the value’s source of truth.

```
struct PlayerView: View {
    var episode: Episode
    @State private var isPlaying: Bool = false

    var body: some View {
        VStack {
            Text(episode.title)
                .foregroundStyle(isPlaying ? .primary : .secondary)
            PlayButton(isPlaying: $isPlaying) // Pass a binding.
        }
    }
}
```

When `PlayerView` initializes `PlayButton`, it passes a binding of its state property into the button’s binding property. Applying the `$` prefix to a property wrapped value returns its projectedValue, which for a state property wrapper returns a binding to the value.

Whenever the user taps the `PlayButton`, the `PlayerView` updates its `isPlaying` state.

A binding conforms to `Sendable` only if its wrapped value type also conforms to `Sendable`. It is always safe to pass a sendable binding between different concurrency domains. However, reading from or writing to a binding’s wrapped value from a different concurrency domain may or may not be safe, depending on how the binding was created. SwiftUI will issue a warning at runtime if it detects a binding being used in a way that may compromise data safety.

Note

To create bindings to properties of a type that conforms to the Observable protocol, use the Bindable property wrapper. For more information, see Migrating from the Observable Object protocol to the Observable macro.

## Topics

### Creating a binding

init(_:)

Creates a binding by projecting the base value to a hashable value.

init(projectedValue: Binding&lt;Value>)

Creates a binding from the value of another binding.

init(get:set:)

Creates a binding with closures that read and write the binding value.

static func constant(Value) -> Binding&lt;Value>

Creates a binding with an immutable value.

### Getting the value

var wrappedValue: Value

The underlying value referenced by the binding variable.

var projectedValue: Binding&lt;Value>

A projection of the binding value that returns a binding.

subscript&lt;Subject>(dynamicMember _: WritableKeyPath&lt;Value, Subject>) -> Binding&lt;Subject>

Returns a binding to the resulting value of a given key path.

### Managing changes

var id: Value.ID

The stable identity of the entity associated with this instance, corresponding to the `id` of the binding’s wrapped value.

func animation(Animation?) -> Binding&lt;Value>

Specifies an animation to perform when the binding value changes.

func transaction(Transaction) -> Binding&lt;Value>

Specifies a transaction for the binding.

var transaction: Transaction

The binding’s transaction.

### Default Implementations

Identifiable Implementations

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- Copyable
- DynamicProperty

  Conforms when `Value` conforms to `Copyable` and `Escapable`.

- Identifiable
- RandomAccessCollection
- Sendable
- Sequence

## See Also

### Creating and sharing view state

Managing user interface state

Encapsulate view-specific data within your app’s view hierarchy to make your views reusable.

struct State

A property wrapper type that can read and write a value managed by SwiftUI.

struct Bindable

A property wrapper type that supports creating bindings to the mutable properties of observable objects.

