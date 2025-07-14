

- TipKit
- Tip
-  Tip.Rule 

Type Alias

# Tip.Rule

A condition to meet before displaying a tip.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
typealias Rule = Tips.Rule
```

## Overview

Use rules to control when your tips display.

### Parameter Rules

Tips.Parameter based rules track app state. For example, to display a tip when someone logs in:

1.  Define the app state you want to track using the `@Parameter` macro.

2.  Define a rule based on that app state using the `#Rule` macro.

3.  Set the conditions for when the tip displays in the macro closure.

```
struct FavoriteLandmarkTip: Tip {
    // Define the app state you want to track.
    @Parameter
    static var userIsLoggedIn: Bool = false

    var rules: [Rule] {
        // Define a rule based on the app state.
        #Rule(Self.$userIsLoggedIn) {
            // Set the conditions for when the tip displays.
            $0 == true
        }
    }
}
```

### Event Rules

Event based rules track user interactions. For example, to display a tip only when a Tips.Event occurs three or more times:

1.  Define the user interaction you want to track as a Tips.Event with a unique `id`.

2.  Define a rule based on that interaction using a `#Rule` macro.

3.  Set the conditions for when the tip displays in the macro closure.

```
struct FavoriteLandmarkTip: Tip {
    // Define the user interaction you want to track.
    static let didViewLandmark: Event = Event(id: "didViewLandmark")

    var rules: [Rule] {
        // Define a rule based on the interaction.
        #Rule(Self.didViewLandmark) {
            // Set the conditions for when the tip displays.
            $0.donations.count > 3
        }
    }
}
```

Note

If no rules are defined within a tip content structure, the tip displays until dismissed or they exceed the threshold of their display frequency.

## Topics

### Creating parameters

struct Parameter

A type that monitors the state of its wrapped value to reevaluate any dependent tip rules when the value changes.

### Creating events and adding donations

struct Event

A repeatable user-defined action.

