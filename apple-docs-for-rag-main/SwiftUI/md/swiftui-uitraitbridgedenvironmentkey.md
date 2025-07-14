

- SwiftUI
-  UITraitBridgedEnvironmentKey 

Protocol

# UITraitBridgedEnvironmentKey

An environment key that is bridged to a UIKit trait.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
protocol UITraitBridgedEnvironmentKey : EnvironmentKey
```

## Overview

Use this protocol to allow the same underlying data to be accessed using an environment key in SwiftUI and trait in UIKit. As the bridging is bidirectional, values written to the trait in UIKit can be read using the environment key in SwiftUI, and values written to the environment key in SwiftUI can be read from the trait in UIKit.

Given a custom UIKit trait named `MyTrait` with `myTrait` properties on both `UITraitCollection` and `UIMutableTraits`:

```
struct MyTrait: UITraitDefinition {
    static let defaultValue = "Default value"
}

extension UITraitCollection {
    var myTrait: String {
        self[MyTrait.self]
    }
}

extension UIMutableTraits {
    var myTrait: String {
        get { self[MyTrait.self] }
        set { self[MyTrait.self] = newValue }
    }
}
```

You can declare an environment key to represent the same data:

```
struct MyEnvironmentKey: EnvironmentKey {
    static let defaultValue = "Default value"
}
```

Bridge the environment key and the trait by conforming to the `UITraitBridgedEnvironmentKey` protocol, providing implementations of read(from:) and write(to:value:) to losslessly convert the environment value from and to the corresponding trait value:

```
extension MyEnvironmentKey: UITraitBridgedEnvironmentKey {
    static func read(
        from traitCollection: UITraitCollection
    ) -> String {
        traitCollection.myTrait
    }

    static func write(
        to mutableTraits: inout UIMutableTraits, value: String
    ) {
        mutableTraits.myTrait = value
    }
}
```

## Topics

### Managing the keys

static func read(from: UITraitCollection) -> Self.Value

Reads the trait value from the trait collection, and returns the equivalent environment value.

**Required**

static func write(to: inout any UIMutableTraits, value: Self.Value)

Writes the equivalent trait value for the environment value into the mutable traits.

**Required**

## Relationships

### Inherits From

- EnvironmentKey

