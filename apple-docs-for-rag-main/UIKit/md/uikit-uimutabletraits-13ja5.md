

- UIKit
-  UIMutableTraits 

Protocol

# UIMutableTraits

A mutable container of traits.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
protocol UIMutableTraits
```

## Overview

The UIMutableTraits protocol provides read-write access to get and set trait values on an underlying container. UIKit uses this protocol to facilitate working with instances of UITraitCollection, which are immutable and read-only. The UITraitCollection initializer init(mutations:) uses an instance of UIMutableTraits, which enables you to set a batch of trait values in one method call. UITraitOverrides conforms to UIMutableTraits, making it easy to set trait overrides on trait environments such as views and view controllers.

When you define a custom trait, declare a property for the trait in an extension to UIMutableTraits so that you can access your custom trait using standard property syntax.

The following example defines an extension and sets the theme on the traitOverrides property:

```
// ThemeTrait conforms to UITraitDefinition, and has a defaultValue type of Theme
extension UIMutableTraits {
    var theme: Theme {
        get { self[ThemeTrait.self] }
        set { self[ThemeTrait.self] = newValue }
    }
}

// Apply an override for the custom theme trait.
view.traitOverrides.theme = .monochrome
```

## Topics

### Defining custom traits

var accessibilityContrast: UIAccessibilityContrast

struct UITraitAccessibilityContrast

var activeAppearance: UIUserInterfaceActiveAppearance

struct UITraitActiveAppearance

var displayGamut: UIDisplayGamut

struct UITraitDisplayGamut

var displayScale: CGFloat

struct UITraitDisplayScale

var forceTouchCapability: UIForceTouchCapability

struct UITraitForceTouchCapability

var horizontalSizeClass: UIUserInterfaceSizeClass

struct UITraitHorizontalSizeClass

var imageDynamicRange: UIImage.DynamicRange

struct UITraitImageDynamicRange

var layoutDirection: UITraitEnvironmentLayoutDirection

struct UITraitLayoutDirection

var legibilityWeight: UILegibilityWeight

struct UITraitLegibilityWeight

var listEnvironment: UIListEnvironment

struct UITraitListEnvironment

var preferredContentSizeCategory: UIContentSizeCategory

struct UITraitPreferredContentSizeCategory

var sceneCaptureState: UISceneCaptureState

struct UITraitSceneCaptureState

var toolbarItemPresentationSize: UINSToolbarItemPresentationSize

struct UITraitToolbarItemPresentationSize

var typesettingLanguage: Locale.Language?

struct UITraitTypesettingLanguage

var userInterfaceIdiom: UIUserInterfaceIdiom

struct UITraitUserInterfaceIdiom

var userInterfaceLevel: UIUserInterfaceLevel

struct UITraitUserInterfaceLevel

var userInterfaceStyle: UIUserInterfaceStyle

struct UITraitUserInterfaceStyle

var verticalSizeClass: UIUserInterfaceSizeClass

struct UITraitVerticalSizeClass

### Subscripts

subscript&lt;T>(T.Type) -> T.Value

**Required**

subscript&lt;T>(T.Type) -> T.Value

**Required**

subscript&lt;T>(T.Type) -> T.Value

**Required**

subscript&lt;T>(T.Type) -> T.Value

**Required**

subscript&lt;T>(T.Type) -> T.Value

**Required**

subscript&lt;T>(T.Type) -> T.Value

**Required**

subscript&lt;T>(T.Type) -> T.Value

**Required**

subscript&lt;T>(T.Type) -> T.Value

**Required**

subscript&lt;T>(T.Type) -> T.Value

**Required**

subscript&lt;T>(T.Type) -> T.Value

**Required**

subscript&lt;T>(T.Type) -> T.Value

**Required**

subscript&lt;T>(T.Type) -> T.Value

**Required**

subscript&lt;T>(T.Type) -> T.Value

**Required**

subscript&lt;T>(T.Type) -> T.Value

**Required**

subscript&lt;T>(T.Type) -> T.Value

**Required**

subscript&lt;T>(T.Type) -> T.Value

**Required**

## Relationships

### Conforming Types

- UITraitOverrides

## See Also

### Related Documentation

convenience init(mutations: (inout any UIMutableTraits) -> Void)

func modifyingTraits((inout any UIMutableTraits) -> Void) -> UITraitCollection

### Adaptivity

Automatic trait tracking

Reduce the need to manually register for trait changes when you use traits within a method or closure that supports automatic trait tracking.

Responding to changing display modes on Apple TV

Change images and resources dynamically when the screen gamut on your device changes.

class UITraitCollection

A collection of data that represents the environment for an individual element in your app’s user interface.

protocol UITraitEnvironment

A set of methods that makes the iOS interface environment available to your app.

protocol UITraitChangeObservable

A type that calls your code in reaction to changes in the trait environment.

protocol UIAdaptivePresentationControllerDelegate

A set of methods that, in conjunction with a presentation controller, determine how to respond to trait changes in your app.

protocol UIContentContainer

A set of methods for adapting the contents of your view controllers to size and trait changes.

