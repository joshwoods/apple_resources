

- UIKit
-  UITraitCollection 

Class

# UITraitCollection

A collection of data that represents the environment for an individual element in your app’s user interface.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
class UITraitCollection
```

## Mentioned in 

Displaying and managing views with a view controller

Building a desktop-class iPad app

## Overview

The traitCollection property of the UITraitEnvironment protocol contains traits that describe the state of various elements of the iOS user interface, such as size class, display scale, and layout direction. Together, these traits compose the UIKit trait environment.

The following classes adopt UITraitEnvironment: UIScreen, UIWindow, UIViewController, UIPresentationController, and UIView. To create an adaptive interface, write code to adjust your app’s layout according to changes in these traits. You access specific trait values using the UITraitCollection horizontalSizeClass, verticalSizeClass, displayScale, and userInterfaceIdiom properties. The UIUserInterfaceSizeClass enumeration defines the values for the horizontal and vertical size class. The display scale is a floating point number. The UIUserInterfaceIdiom enumeration defines the values for the user interface idiom.

To make your view controllers and views responsive to changes in the iOS interface environment, override the traitCollectionDidChange(_:) method from the trait environment protocol. To customize view controller animations in response to interface environment changes, override the willTransition(to:with:) method of the UIContentContainer protocol.

The following image shows the horizontal (width) and vertical (height) size classes your app can encounter when running full-screen on various devices.

For information about size classes your app encounters in Slide Over and Split View on iPad, read Slide Over and Split View Quick Start in Adopting Multitasking Enhancements on iPad.

You can create standalone trait collections to assist in matching against specific environments. The UITraitCollection class includes four specialized constructors, as well as a constructor that enables you to combine an array of trait collections, init(traitsFrom:).

One important use of standalone trait collections is to enable conditional use of images based on the current iOS interface environment. You can associate a trait collection with a UIImage instance by way of a UIImageAsset instance, as described in the overview section of UIImageAsset. For information on configuring asset catalogs graphically from within the Xcode IDE, see Managing assets with asset catalogs.

You can employ a standalone trait collection to enable a two-column split view in landscape orientation on iPhone. See the setOverrideTraitCollection(_:forChild:) method of the UIViewController class.

You can also use a standalone trait collection to customize view appearance with the appearance(for:) protocol method, as described in UIAppearance.

### 3D Touch and trait collections

Starting in iOS 9, you can use this class to check whether the device on which your app is running supports 3D Touch. Read the value of the forceTouchCapability property on the trait collection for any object in your app with a trait environment. For information about trait environments, see UITraitEnvironment. For the possible values of the force touch capability property, see the UIForceTouchCapability enumeration.

Because a user can turn off 3D Touch in Settings, check the value of the forceTouchCapability property in your implementation of the traitCollectionDidChange(_:) method, and adjust your code paths according to the property’s value.

### Custom traits

You can create a custom trait using UITraitDefinition. You read custom traits from UITraitCollection using subscript syntax. When you define a custom trait, declare a property for the trait in an extension to UITraitCollection so that you can access your custom trait using standard property syntax.

The following example defines a property for a custom trait, and reads the trait value from a trait collection.

```
// ThemeTrait conforms to UITraitDefinition, with a defaultValue type of Theme.
extension UITraitCollection {
    var theme: Theme {
        self[ThemeTrait.self]
    }
}

let viewTheme = view.traitCollection.theme
```

## Topics

### Creating a trait collection

init()

Creates a trait collection whose traits are set to their default (unspecified) values.

init(userInterfaceIdiom: UIUserInterfaceIdiom)

Creates a trait collection that contains only a specified interface idiom.

init(horizontalSizeClass: UIUserInterfaceSizeClass)

Creates a trait collection that contains only a specified horizontal size class.

init(verticalSizeClass: UIUserInterfaceSizeClass)

Creates a trait collection that contains only a specified vertical size class.

init(userInterfaceStyle: UIUserInterfaceStyle)

Creates a trait collection that contains only the specified user interface style trait.

init(accessibilityContrast: UIAccessibilityContrast)

Creates a trait collection that contains only the specified accessibility contrast trait.

init(userInterfaceLevel: UIUserInterfaceLevel)

Creates a trait collection that contains only the specified user interface level trait.

init(legibilityWeight: UILegibilityWeight)

Creates a trait collection that contains only the specified legibility weight trait.

init(forceTouchCapability: UIForceTouchCapability)

Creates a trait collection that contains only a specified force touch capability trait.

init(displayScale: CGFloat)

Creates a trait collection that contains only a specified display scale.

init(displayGamut: UIDisplayGamut)

Creates a trait collection that contains only the specified display gamut trait.

init(layoutDirection: UITraitEnvironmentLayoutDirection)

Creates a trait collection that contains only the specified layout direction trait.

init(preferredContentSizeCategory: UIContentSizeCategory)

Creates a trait collection that contains only the specified content size category trait.

init(activeAppearance: UIUserInterfaceActiveAppearance)

Creates a trait collection that contains only the specified active appearance trait.

init(toolbarItemPresentationSize: UINSToolbarItemPresentationSize)

Creates a trait collection that contains only the specified toolbar item presentation size trait.

init?(coder: NSCoder)

Creates a trait collection from data in an unarchiver.

init(traitsFrom: [UITraitCollection])

Creates a trait collection that consists of traits merged from a specified array of trait collections.

Deprecated

### Modifying traits

convenience init(mutations: (inout any UIMutableTraits) -> Void)

func modifyingTraits((inout any UIMutableTraits) -> Void) -> UITraitCollection

typealias TraitMutations

### Getting the current traits

class var current: UITraitCollection

The trait collection for the current execution context.

### Retrieving size class traits

var horizontalSizeClass: UIUserInterfaceSizeClass

The horizontal size class of the trait collection.

var verticalSizeClass: UIUserInterfaceSizeClass

The vertical size class of the trait collection.

enum UIUserInterfaceSizeClass

Constants that indicate the size class of a view.

### Retrieving display-related traits

var displayScale: CGFloat

The display scale of the trait collection.

var displayGamut: UIDisplayGamut

The gamut of the current display.

enum UIDisplayGamut

Constants that indicate the gamut of the current display.

### Retrieving interface-related traits

var userInterfaceStyle: UIUserInterfaceStyle

The style associated with the user interface.

enum UIUserInterfaceStyle

Constants that indicate the interface style for the app.

var userInterfaceIdiom: UIUserInterfaceIdiom

The user interface idiom of the trait collection.

enum UIUserInterfaceIdiom

Constants that indicate the interface type for the device or an object that has a trait environment, such as a view and view controller.

var userInterfaceLevel: UIUserInterfaceLevel

The elevation level of the interface.

enum UIUserInterfaceLevel

Constants that indicate the visual level for content in the window.

var layoutDirection: UITraitEnvironmentLayoutDirection

The layout direction associated with the current environment.

enum UITraitEnvironmentLayoutDirection

Constants that indicate the layout direction associated with the current environment.

var accessibilityContrast: UIAccessibilityContrast

The accessibility contrast associated with the current environment.

enum UIAccessibilityContrast

Constants that indicate the accessibility contrast setting.

var legibilityWeight: UILegibilityWeight

The font weight to apply to text.

enum UILegibilityWeight

Constants that indicate the weight to apply to text in your interface.

var activeAppearance: UIUserInterfaceActiveAppearance

A property that indicates whether the user interface has an active appearance.

enum UIUserInterfaceActiveAppearance

Constants that indicate whether the user interface has an active appearance.

var toolbarItemPresentationSize: UINSToolbarItemPresentationSize

The presentation size of a toolbar item in an AppKit toolbar.

enum UINSToolbarItemPresentationSize

Constants that specify the presentation size of a toolbar item in an AppKit toolbar.

### Retrieving the force touch capability traits

var forceTouchCapability: UIForceTouchCapability

The force touch capability value of the trait collection.

enum UIForceTouchCapability

Keys that indicate the availability of 3D Touch on a device.

### Retrieving content size category information

var preferredContentSizeCategory: UIContentSizeCategory

The font sizing option preferred by the user.

struct UIContentSizeCategory

Constants that indicate the preferred size of your content.

### Retrieving list environment traits

var listEnvironment: UIListEnvironment

enum UIListEnvironment

Constants that indicate the style of the containing list in a collection view or table view.

### Retrieving scene capture state

var sceneCaptureState: UISceneCaptureState

enum UISceneCaptureState

### Retrieving dynamic range traits

var imageDynamicRange: UIImage.DynamicRange

### Retrieving typesetting language traits

var typesettingLanguage: Locale.Language?

### Comparing trait collections

func hasDifferentColorAppearance(comparedTo: UITraitCollection?) -> Bool

Queries whether changing between the specified and current trait collections would affect color values.

func containsTraits(in: UITraitCollection?) -> Bool

Queries whether a trait collection contains all of another trait collection’s values.

Deprecated

### Getting an image configuration object

var imageConfiguration: UIImage.Configuration

An image configuration object compatible with this trait collection.

### Performing actions with the current traits

func performAsCurrent(() -> Void)

Executes custom code using the traits of the receiving trait collection.

### Initializers

convenience init&lt;T>(T.Type, value: T.Value)

convenience init&lt;T>(T.Type, value: T.Value)

convenience init&lt;T>(T.Type, value: T.Value)

convenience init&lt;T>(T.Type, value: T.Value)

convenience init&lt;T>(T.Type, value: T.Value)

convenience init&lt;T>(T.Type, value: T.Value)

convenience init&lt;T>(T.Type, value: T.Value)

convenience init&lt;T>(T.Type, value: T.Value)

convenience init&lt;T>(T.Type, value: T.Value)

convenience init&lt;T>(T.Type, value: T.Value)

convenience init&lt;T>(T.Type, value: T.Value)

convenience init&lt;T>(T.Type, value: T.Value)

convenience init&lt;T>(T.Type, value: T.Value)

convenience init&lt;T>(T.Type, value: T.Value)

convenience init&lt;T>(T.Type, value: T.Value)

convenience init&lt;T>(T.Type, value: T.Value)

init(imageDynamicRange: UIImage.DynamicRange)

init(listEnvironment: UIListEnvironment)

init(sceneCaptureState: UISceneCaptureState)

convenience init(typesettingLanguage: Locale.Language?)

### Instance Methods

func changedTraits(from: UITraitCollection?) -> [UITrait]

func replacing&lt;T>(T.Type, value: T.Value) -> UITraitCollection

func replacing&lt;T>(T.Type, value: T.Value) -> UITraitCollection

func replacing&lt;T>(T.Type, value: T.Value) -> UITraitCollection

func replacing&lt;T>(T.Type, value: T.Value) -> UITraitCollection

func replacing&lt;T>(T.Type, value: T.Value) -> UITraitCollection

func replacing&lt;T>(T.Type, value: T.Value) -> UITraitCollection

func replacing&lt;T>(T.Type, value: T.Value) -> UITraitCollection

func replacing&lt;T>(T.Type, value: T.Value) -> UITraitCollection

func replacing&lt;T>(T.Type, value: T.Value) -> UITraitCollection

func replacing&lt;T>(T.Type, value: T.Value) -> UITraitCollection

func replacing&lt;T>(T.Type, value: T.Value) -> UITraitCollection

func replacing&lt;T>(T.Type, value: T.Value) -> UITraitCollection

func replacing&lt;T>(T.Type, value: T.Value) -> UITraitCollection

func replacing&lt;T>(T.Type, value: T.Value) -> UITraitCollection

func replacing&lt;T>(T.Type, value: T.Value) -> UITraitCollection

func replacing&lt;T>(T.Type, value: T.Value) -> UITraitCollection

### Subscripts

subscript&lt;T>(T.Type) -> T.Value

subscript&lt;T>(T.Type) -> T.Value

subscript&lt;T>(T.Type) -> T.Value

subscript&lt;T>(T.Type) -> T.Value

subscript&lt;T>(T.Type) -> T.Value

subscript&lt;T>(T.Type) -> T.Value

subscript&lt;T>(T.Type) -> T.Value

subscript&lt;T>(T.Type) -> T.Value

subscript&lt;T>(T.Type) -> T.Value

subscript&lt;T>(T.Type) -> T.Value

subscript&lt;T>(T.Type) -> T.Value

subscript&lt;T>(T.Type) -> T.Value

subscript&lt;T>(T.Type) -> T.Value

subscript&lt;T>(T.Type) -> T.Value

subscript&lt;T>(T.Type) -> T.Value

subscript&lt;T>(T.Type) -> T.Value

### Type Properties

static var systemTraitsAffectingColorAppearance: [UITrait]

static var systemTraitsAffectingImageLookup: [UITrait]

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Adaptivity

Automatic trait tracking

Reduce the need to manually register for trait changes when you use traits within a method or closure that supports automatic trait tracking.

Responding to changing display modes on Apple TV

Change images and resources dynamically when the screen gamut on your device changes.

protocol UITraitEnvironment

A set of methods that makes the iOS interface environment available to your app.

protocol UITraitChangeObservable

A type that calls your code in reaction to changes in the trait environment.

protocol UIMutableTraits

A mutable container of traits.

protocol UIAdaptivePresentationControllerDelegate

A set of methods that, in conjunction with a presentation controller, determine how to respond to trait changes in your app.

protocol UIContentContainer

A set of methods for adapting the contents of your view controllers to size and trait changes.

