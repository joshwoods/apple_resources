

- SwiftUI
-  EmptyModifier 

Structure

# EmptyModifier

An empty, or identity, modifier, used during development to switch modifiers at compile time.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct EmptyModifier
```

## Overview

Use the empty modifier to switch modifiers at compile time during development. In the example below, in a debug build the Text view inside `ContentView` has a yellow background and a red border. A non-debug build reflects the default system, or container supplied appearance.

```
struct EmphasizedLayout: ViewModifier {
    func body(content: Content) -> some View {
        content
            .background(Color.yellow)
            .border(Color.red)
    }
}

struct ContentView: View {
    var body: some View {
        Text("Hello, World!")
            .modifier(modifier)
    }

    var modifier: some ViewModifier {
        #if DEBUG
            return EmphasizedLayout()
        #else
            return EmptyModifier()
        #endif
    }
}
```

## Topics

### Creating an empty modifier

init()

### Getting the identity modifier

static let identity: EmptyModifier

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Sendable
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

struct ModifiedContent

A value with a modifier applied to it.

protocol EnvironmentalModifier

A modifier that must resolve to a concrete modifier in an environment before use.

