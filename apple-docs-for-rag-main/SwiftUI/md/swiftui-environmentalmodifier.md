

- SwiftUI
-  EnvironmentalModifier 

Protocol

# EnvironmentalModifier

A modifier that must resolve to a concrete modifier in an environment before use.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol EnvironmentalModifier : ViewModifier where Self.Body == Never
```

## Topics

### Resolving a modifier

func resolve(in: EnvironmentValues) -> Self.ResolvedModifier

Resolve to a concrete modifier in the given `environment`.

**Required**

associatedtype ResolvedModifier : ViewModifier

The type of modifier to use after being resolved.

**Required**

## Relationships

### Inherits From

- ViewModifier

## See Also

### Modifying a view

Configuring views

Adjust the characteristics of a view by applying view modifiers.

Reducing view modifier maintenance

Bundle view modifiers that you regularly reuse into a custom view modifier.

func modifier&lt;T>(T) -> ModifiedContent&lt;Self, T>

Applies a modifier to a view and returns a new view.

protocol ViewModifier

A modifier that you apply to a view or another view modifier, producing a different version of the original value.

struct EmptyModifier

An empty, or identity, modifier, used during development to switch modifiers at compile time.

struct ModifiedContent

A value with a modifier applied to it.

