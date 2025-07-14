

- SwiftUI
-  OpenImmersiveSpaceAction 

Structure

# OpenImmersiveSpaceAction

An action that presents an immersive space.

visionOS 1.0+

``` source
@MainActor
struct OpenImmersiveSpaceAction
```

## Overview

Use the openImmersiveSpace environment value to get the instance of this structure for a given Environment. Then call the instance to present a space. You call the instance directly because it defines `callAsFunction()` methods that Swift calls when you call the instance.

For example, you can define a button that opens a specified planet in an immersive space:

```
@main
struct SolarSystemApp: App {
    var body: some Scene {
        ImmersiveSpace(for: Planet.ID.self) { $planetID in
            // ...
        }
    }
}

struct ShowPlanetButton: View {
    var planet: Planet
    @Environment(\.openImmersiveSpace) private var openImmersiveSpace

    var body: some View {
        Button("Show \(planet.name)") {
            Task {
                await openImmersiveSpace(value: planet.ID)
            }
        }
    }
}
```

You indicate which immersive space to open by providing one of the following:

- A string identifier that you pass through the `id` parameter.

- A `value` parameter that has a type that matches the type that you specify in the space’s initializer, as in the above example.

- Both an identifier and a value. This enables you to define multiple spaces that take input values of the same type and distinguish them by their string identifiers.

The call is asynchronous and returns after presenting the space or if an error occurs. You can check for errors by inspecting the call’s return value, which is of type OpenImmersiveSpaceAction.Result. For example, the call returns an error if you already have an immersive space open, because the system enables only one space to be open at a time.

If you provide a value when you open the space, the scene’s trailing closure receives a binding to the value that you provide. For best performance, use lightweight data for the presentation value. For structured model values that conform to Identifiable, the value’s identifier makes a good presentation value, like the `planet.ID` value in the above code.

## Topics

### Calling the action

func callAsFunction(id: String) async -> OpenImmersiveSpaceAction.Result

Presents an immersive space for the scene with the specified identifier.

func callAsFunction&lt;D>(id: String, value: D) async -> OpenImmersiveSpaceAction.Result

Presents the immersive space that your app defines for the specified identifier and that handles the type of the presented value.

func callAsFunction&lt;D>(value: D) async -> OpenImmersiveSpaceAction.Result

Presents the immersive space that handles the type of the presented value.

### Getting the result

enum Result

The outcome of an attempt to open an immersive space.

## Relationships

### Conforms To

- Sendable

## See Also

### Opening an immersive space

var openImmersiveSpace: OpenImmersiveSpaceAction

An action that presents an immersive space.

