

- UIKit
-  UIBarAppearance 

Class

# UIBarAppearance

An object for customizing the basic appearance of system bars.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class UIBarAppearance
```

## Overview

A UIBarAppearance object contains the common traits shared by navigation bars, tab bars, and toolbars. When configuring a specific type of bar, you usually instantiate the appropriate bar appearance subclass. However, you may also create a UIBarAppearance object, configure its properties, and use it to create new bar appearance objects in your app.

## Topics

### Creating a custom bar appearance object

init(idiom: UIUserInterfaceIdiom)

Creates a new bar appearance object that targets the specified idiom.

init(barAppearance: UIBarAppearance)

Creates a new bar appearance object by copying relevant data from the specified appearance object.

convenience init()

Creates a new bar appearance object containing default values.

init(coder: NSCoder)

Creates an appearance object from data in an unarchiver.

### Copying a custom bar appearance object

func copy() -> Self

Creates a copy of the appearance object.

### Resetting the appearance properties

func configureWithDefaultBackground()

Configures the bar appearance object with default background and shadow values.

func configureWithOpaqueBackground()

Configures the bar appearance object with a set of opaque colors that are appropriate for the current theme.

func configureWithTransparentBackground()

Configures the bar appearance object with a transparent background and no shadow.

### Configuring the background appearance

var backgroundEffect: UIBlurEffect?

The blur effect to apply to the bar’s background.

var backgroundColor: UIColor?

The background color of the bar.

var backgroundImage: UIImage?

The image to display on top of the bar’s background color.

var backgroundImageContentMode: UIView.ContentMode

The content mode to use when displaying the bar’s background image.

### Configuring the shadow appearance

var shadowColor: UIColor?

The color to apply to the bar’s custom or default shadow.

var shadowImage: UIImage?

The image to use for the bar’s shadow.

### Getting the supported idiom

var idiom: UIUserInterfaceIdiom

The idiom targeted by this bar appearance object.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UINavigationBarAppearance
- UITabBarAppearance
- UIToolbarAppearance

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

### Shared appearance

class UIBarButtonItemAppearance

An object for customizing the appearance of bar button items.

class UIBarButtonItemStateAppearance

A data object containing the specific customizations for a bar button item in a particular state.

