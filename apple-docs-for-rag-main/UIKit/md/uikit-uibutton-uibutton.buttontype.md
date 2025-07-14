

- UIKit
- UIButton
-  UIButton.ButtonType 

Enumeration

# UIButton.ButtonType

Specifies the style of a button.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum ButtonType
```

## Topics

### Constants

case custom

No button style.

case system

A system style button, such as those shown in navigation bars and toolbars.

case detailDisclosure

A detail disclosure button.

case infoLight

An information button that has a light background.

case infoDark

An information button that has a dark background.

case contactAdd

A contact add button.

case plain

A standard system button without a blurred background view.

case close

A close button to dismiss panels and views.

static var roundedRect: UIButton.ButtonType

A rounded-rectangle style button.

Deprecated

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating buttons of a specific type

convenience init(type: UIButton.ButtonType)

Creates and returns a new button of the specified type.

convenience init(type: UIButton.ButtonType, primaryAction: UIAction?)

Creates a new button with the specified type, registers the primary action event, and sets the title and image to the action’s title and image.

