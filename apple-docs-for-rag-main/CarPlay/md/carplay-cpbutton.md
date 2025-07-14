

- CarPlay
-  CPButton 

Class

# CPButton

A button that displays an image and invokes a handler when the user taps it.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class CPButton
```

## Overview

You create instances of `CPButton` to provide a template’s actions. The button displays a custom image that communicates its function. When a user taps the button, CarPlay invokes the handler you provide. The template that contains the button manages its appearance.

The framework provides specialized subclasses for common actions, such as CPContactCallButton or CPContactMessageButton.

## Topics

### Creating a Button

init(image: UIImage, handler: ((CPButton) -> Void)?)

Creates a button that displays an image and invokes a handler when the user taps it.

let CPButtonMaximumImageSize: CGSize

The maximum size of a button’s image that CarPlay supports.

### Getting the Button’s Image

var image: UIImage?

The button’s image.

### Configuring the Button’s Attributes

var title: String?

The button’s title.

var isEnabled: Bool

A Boolean value that determines whether the button is in an enabled state.

## Relationships

### Inherits From

- NSObject

### Inherited By

- CPContactCallButton
- CPContactDirectionsButton
- CPContactMessageButton

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Related Types

class CPImageSet

Light and dark representations of an image.

let CarPlayErrorDomain: String

The domain that CarPlay uses for any errors it provides.

