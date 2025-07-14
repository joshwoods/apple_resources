

- UIKit
-  UITraitDefinition 

Protocol

# UITraitDefinition

A type representing a trait in a trait collection.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
protocol UITraitDefinition
```

## Overview

All traits contained in a UITraitCollection conform to this protocol. You can create custom traits by defining your own conforming type.

The example below defines a new trait that holds the value of an integer-based enumeration named `Theme`:

```
enum Theme: Int {
    case standard
    case monochrome
}

struct ThemeTrait: UITraitDefinition {
    static let defaultValue = Theme.standard
}
```

The protocol defines default implementations for name and identifier properties. Defining defaultValue is the minimum requirement to conform to this protocol. All properties you implement must be constant. `UITraitDefinition` defines the associated type Value which is the type of defaultValue.

The best candidates for trait values are simple value types, such as Bool, Int, Double, and enumerations with an Int raw value. You can also use lightweight structures as trait values. The system frequently tests trait values for equality, so structures need an efficient implementation of `Equatable`. Avoid using Swift classes as trait values.

If you use your custom trait to implement custom dynamic colors, implement affectsColorAppearance and return `true`. Returning `true` tells the system to update and redraw views automatically when the trait changes. The system responds to changes to your trait similar to changes in system traits contained in systemTraitsAffectingColorAppearance. Changes to traits that affect color appearance are more expensive, so opt in to this behavior only when necessary, and change such traits infrequently.

For each custom trait, define extensions on UIMutableTraits and UITraitCollection to enable reading and modifying your custom traits with standard property syntax. The example below shows extensions for the example `Theme` trait.

```
extension UITraitCollection {
    var theme: Theme { self[ThemeTrait.self] }
}

extension UIMutableTraits {
    var theme: Theme {
        get { self[ThemeTrait.self] }
        set { self[ThemeTrait.self] = newValue }
    }
}
```

A trait type serves as a unique key, identifying a trait within a trait collection. Methods such as subscript(_:) and `UIPresentationController/registerForTraitChanges(_:handler:)` take a trait type to identify the trait in a collection.

Traits defined in Swift aren’t automatically bridged to Objective-C. If you need to access your custom trait from both Swift and Objective-C code, define the trait in both languages. For details, see the Objective-C documentation for UITraitDefinition.

## Topics

### Associated Types

associatedtype Value

**Required**

### Type Properties

static var affectsColorAppearance: Bool

**Required** Default implementation provided.

static var defaultValue: Self.Value

**Required**

static var identifier: String

**Required** Default implementation provided.

static var name: String

**Required** Default implementation provided.

## Relationships

### Conforming Types

- UITraitAccessibilityContrast
- UITraitActiveAppearance
- UITraitDisplayGamut
- UITraitDisplayScale
- UITraitForceTouchCapability
- UITraitHorizontalSizeClass
- UITraitImageDynamicRange
- UITraitLayoutDirection
- UITraitLegibilityWeight
- UITraitListEnvironment
- UITraitPreferredContentSizeCategory
- UITraitSceneCaptureState
- UITraitToolbarItemPresentationSize
- UITraitTypesettingLanguage
- UITraitUserInterfaceIdiom
- UITraitUserInterfaceLevel
- UITraitUserInterfaceStyle
- UITraitVerticalSizeClass

## See Also

### Custom traits

protocol UIMutableTraits

A mutable container of traits.

typealias UITrait

A type representing a trait in a trait collection.

